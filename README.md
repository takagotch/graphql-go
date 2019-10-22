### graphql-go
---
https://github.com/graph-gophers/graphql-go

https://github.com/tmc/graphql

https://github.com/graphql-go/graphql

```go
// introspection_test.go

func TestSchema_ToJSON(t *testing.T) {
  t.Parallel()
  
  type args struct {
    Schema *graphql.Schema
  }
  type want struct {
    JSON []byte
  }
}


```

```go
// parser/parser_test.go

func TestMalformedQuery(t *testing.T) {
  op, err := parser.ParseOpenration(nil)
  if !parser.IsMalformedOperation(err) {
    t.Error("Expected malformed operation")
  }
  
}

func TestMultipleOperations(t *testing.T) {
  multi := `
  `
  op, err := parser.ParseOperation([]byte(mulit))
  if err != parser.ErrMultipleOperations {
    t.Error("Expected multiple operatoins error")
  }
  if op != nil {
    t.Error("Expected nil result")
  }
}


```

```
//

```


