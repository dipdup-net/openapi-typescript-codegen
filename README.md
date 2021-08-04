# OpenAPI Typescript Codegen with TzKT extensions

This is an extended version of the original library by [Ferdi Koomen](https://github.com/ferdikoomen/openapi-typescript-codegen) with TzKT-specific features:
* Query selectors `?field.eq=12345`
* Anyof selector `?anyof.initiator.sender=KT1abcde`
* JSON filters `?storage.ledger.[*].eq=12345`
* Better handling NSwag generated spec (tag prefix removed from operationId)

In addition to that, OpenAPI singleton is removed (thanks to [Craig McNicholas](https://github.com/yottaltd/openapi-typescript-codegen)) so that you can have multiple instances of a service.

## Installation

```
yarn add -D @dipdup/openapi-typescript-codegen
```


## Code generation

```
openapi --useOptions --useUnionTypes --input spec.json --output ./src
```
