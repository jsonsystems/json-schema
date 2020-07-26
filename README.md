# Welcome to JSONschema.Net

[![Hex.pm](https://img.shields.io/hexpm/l/plug.svg)]()

1.  [Contact](#contact)
2.  [What is JSONSchema.Net?](#what-is-jsonschemanet)
3.  [Who uses JSONSchema.Net?](#who-uses-jsonschemanet)
4.  [What is JSONSchema.Net’s goal?](#what-is-jsonschemanets-goal)
5.  [How can your organization benefit from using JSONSchema.Net?](#how-can-your-organization-benefit-from-using-jsonschemanet)
6.  [Specifications](#specifications)
7.  [About](#about)
8.  [Cookie Policy](#cookie)
9.  [Privacy Policy](#privacy-policy)

### Contact

- Email: info@jsonschema.net

### What is JSONSchema.Net?

[JSONSchema.Net](https://www.jsonschema.net) is a web application that generates JSON schema from JSON. JSON Schema is generated according to
the [JSON Schema Validation: A Vocabulary for Structural Validation of JSON](http://json-schema.org/latest/json-schema-validation.html).

### Who uses JSONSchema.Net?

Anyone wishing to generate JSON schema from JSON. Typical users are web developers and mobile app developers. Some educational institutions also use [JSONSchema.Net](https://www.jsonschema.net) to teach JSON Schema and the core options defined by [JSON Schema Validation](http://json-schema.org/latest/json-schema-validation.html).

### What is JSONSchema.Net’s goal?

JSON Schema is great, but can be verbose. For example, a single empty JSON object, `{}`, can be described by:

```
{
  "$schema": "http://json-schema.org/draft-04/schema#",
  "additionalProperties": true,
  "definitions": {},
  "id": "http://example.com/example.json",
  "properties": {
    "description": "This accepts anything, as long as it's valid JSON.",
    "title": "Empty Object"
  },
  "type": [
    "object",
    "null"
  ]
}
```

Even schemas for small APIs can quickly become hundreds of lines long. Writing schemas by hand is tedious and time consuming, and often impractical. JSONSchema.Net makes schema generation quick and painless.

### How can your organization benefit from using JSONSchema.Net?

[JSONSchema.Net](https://www.jsonschema.net) can save you and anyone on your team a lot of time. If your software uses JSON, it's good practice to validate any (JSON) data it receives, against a schema.

### Specifications

JSON Schema specificaiton is split into three parts

1.  Core - The basic foundation of JSON Schema.
2.  Validation - The validation keywords of JSON Schema.
3.  Hyper-Schema - The hyper-media keywords of JSON Schema.

JSONSchema.Net follows the Validation part of the overall specification. [json-schema.org/specification.html](http://json-schema.org/specification.html) is a good place to learning more.

Versioning of JSON Schema specifications can be confusing. [json-schema.org](http://json-schema.org) maintains a helpful list of [specification-links](http://json-schema.org/specification-links.html). In reverse chronological order:

- Latest Snapshot (work in progress)
- Draft 7
- Draft 6
- Draft 5
- Draft 4
- Draft 3
- Drafts 0/1/2

Each version updates (to varying degrees) the three parts of JSON Schema specification: Core, Validation, and Hyper-Schema.

### About

Created by Jack Wootton. Copyright 2017. Apache Licensed.

### Cookie
Our cookie policy can be read at [cookies.md](https://github.com/jsonsystems/json-schema/blob/master/cookies.md)

### Privacy
Our privacy policy can be read at [privacy.md](https://github.com/jsonsystems/json-schema/blob/master/privacy.md)
