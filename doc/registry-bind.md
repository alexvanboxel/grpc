GRPC and Proto Registry Bind Protocol
=====================================

This document describes a standardized registry protocol. 

## Use cases

## Service Definition

The server should export a service defined in the following proto:

```
package grpc.registry.v1alpha1;

service Bind {
    rpc CreateResourceBinding (CreateResourceBindingRequest) returns (CreateResourceBindingResponse);
    rpc UpdateResourceBinding (UpdateResourceBindingRequest) returns (UpdateResourceBindingResponse);
    rpc DeleteResourceBinding (DeleteResourceBindingRequest) returns (DeleteResourceBindingResponse);
    rpc GetResourceBinding (GetResourceBindingeRequest) returns (GetResourceBindingResponse);
    rpc ListResourceBindings (ListResourceBindingsRequest) returns (ListResourceBindingsResponse);
    rpc UseResource (UseResourceRequest) returns (UseResourceResponse);
}
```

