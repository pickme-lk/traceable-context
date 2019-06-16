## Traceable Context

**Traceable Context** is a wrapper around go context which will provide a way to share a traceable UUID between 
different contexts  


* New context
```go
    ctx := traceable_context.WithUUID(uuid.New())
```

* Context from a parent context
```go
    parent := contect.Background()
    ctx := traceable_context.WithUUID(parent, uuid.New())
```
