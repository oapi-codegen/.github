# oapi-codegen

Community organisation for the Go OpenAPI code generator, [oapi-codegen/oapi-codegen](https://github.com/oapi-codegen/oapi-codegen) and its related projects.

## Projects

`oapi-codegen` is primarily operated out of two core projects:

- [oapi-codegen/oapi-codegen](https://github.com/oapi-codegen/oapi-codegen)
- [oapi-codegen/runtime](https://github.com/oapi-codegen/runtime)

Additionally, there are the following HTTP middleware bindings for performing request/response validation against the OpenAPI spec: 

- [oapi-codegen/nethttp-middleware](https://github.com/oapi-codegen/nethttp-middleware)
- [oapi-codegen/fiber-middleware](https://github.com/oapi-codegen/fiber-middleware)
- [oapi-codegen/iris-middleware](https://github.com/oapi-codegen/iris-middleware)
- [oapi-codegen/echo-middleware](https://github.com/oapi-codegen/echo-middleware)
- [oapi-codegen/gin-middleware](https://github.com/oapi-codegen/gin-middleware)

## Non-OpenAPI projects

Additionally, there is [the `nullable` package](https://github.com/oapi-codegen/nullable):

> An implementation of a `Nullable` type for JSON bodies, indicating whether the field is absent, set to `null`, or set to a value

And the lesser used `testutil` project, which can provide a more fluent means to create HTTP requests, and validate them:

- [oapi-codegen/testutil](https://github.com/oapi-codegen/testutil)
