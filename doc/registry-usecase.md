GRPC and Proto Registry Use Cases
=================================

This document describes a standardized registry protocol. 

## Use cases



## Service Definition

The server should export a service defined in the following proto:

```
package grpc.registry.v1alpha1;

service Registry {
    rpc GetSchema (GetSchemaRequest) returns (GetSchemaResponse);
    rpc VerifySchema (SubmitSchemaRequest) returns (SubmitSchemaResponse);
    rpc SubmitSchema (SubmitSchemaRequest) returns (SubmitSchemaResponse);
    rpc VerifyPatch (PatchSchemaRequest) returns (PatchSchemaResponse);
    rpc PatchSchema (PatchSchemaRequest) returns (PatchSchemaResponse);
}
```

