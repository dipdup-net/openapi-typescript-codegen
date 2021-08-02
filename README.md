# OpenAPI Typescript Codegen with TzKT extensions

This is an extended version of the [original library](https://github.com/ferdikoomen/openapi-typescript-codegen) by Ferdi Koomen extended with TzKT-specific features:
* Query selectors `?field.eq=12345`
* Anyof selector `?anyof.initiator.sender=KT1abcde`
* JSON filters `?storage.ledger.[*].eq=12345`

In addition to that, OpenAPI singleton is removed (thanks to [Craig McNicholas](https://github.com/yottaltd/openapi-typescript-codegen)).

## Installation

```
yarn add -D @baking-bad/openapi-typescript-codegen
```


## Code generation

```
openapi --useOptions --useUnionTypes --input spec.json --output ./src
```
