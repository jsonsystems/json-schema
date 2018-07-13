Welcome to JSONschema.Net
=========================
[<img src="https://us-central1-json-schema.cloudfunctions.net/function-1">]
[<img src="https://img.shields.io/badge/donate-paypal-brightgreen.svg">](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=YDKCU75EK795U)
[![Hex.pm](https://img.shields.io/hexpm/l/plug.svg)]()
[![Twitter Follow](https://img.shields.io/twitter/follow/espadrine.svg?style=social&label=Follow)](https://twitter.com/jsonschema)

1. [Contact](#contact)
2. [Donate](#donate)
3. [What is JSONSchema.Net?](#what-is-jsonschemanet)
4. [How does JSONSchema.Net work?](#how-does-jsonschemanet-work)
5. [Who uses JSONSchema.Net?](#who-uses-jsonschemanet)
6. [What is JSONSchema.Net’s goal?](#what-is-jsonschemanets-goal)
7. [How can your organization benefit from using JSONSchema.Net?](#how-can-your-organization-benefit-from-using-jsonschemanet)
8. [Gallery](#gallery)
9. [Specifications](#specifications)


### Contact
* Email: info@jsonschema.net
* Twitter: [@jsonschema](https://twitter.com/jsonschema)


### Donate

[<img src="https://img.shields.io/badge/donate-paypal-brightgreen.svg">](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=YDKCU75EK795U)

JSONSchema.Net is designed to save you time and make your day a little easier.

There are no adverts and no login is required. Nothing is logged beyond default application server logs and there are no tracking pixels other than Google Analytics.

Your JSON is never stored and you're always secured with 256 bit encryption.

If you find JSONSchema.Net useful, please consider [donating to help](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=YDKCU75EK795U) with the cost of:

* Application server uptime
* Web server uptime
* SSL certificates

### What is JSONSchema.Net?
[JSONSchema.Net](https://www.jsonschema.net) is a web application that generates JSON schema from JSON.  JSON Schema is generated according to
the [JSON Schema Validation: A Vocabulary for Structural Validation of JSON](http://json-schema.org/latest/json-schema-validation.html).

### How does JSONSchema.Net work?
Users' interact with JSONSchema.Net using a web *frontend* written in [Angular](https://angular.io). The *backend* is written in Python and runs on Google's Compute Engine in their Cloud.  An [NGINX](https://www.nginx.com/resources/wiki/) reverse proxy sits between the backend and the frontend - primarily to transcode JSON to [Protocol Buffers](https://developers.google.com/protocol-buffers/) and vice-versa.

[Cloud Endpoints: Architectural Overview](https://cloud.google.com/endpoints/docs/grpc/architecture-overview) provides a high-level view of [Cloud Endpoints Architecture](https://cloud.google.com/endpoints/docs/grpc/architecture-overview#cloud_endpoints_architecture), and thus, the architecture of JSONSchema.Net.

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

### Gallery
![JSON Schema](media/1.png?raw=true "JSON Schema")

### Specifications
JSON Schema specificaiton is split into three parts

1. Core - The basic foundation of JSON Schema.
2. Validation - The validation keywords of JSON Schema.
3. Hyper-Schema - The hyper-media keywords of JSON Schema.

JSONSchema.Net follows the Validation part of the overall specification. [json-schema.org/specification.html](http://json-schema.org/specification.html) is a good place to learning more.

Versioning of JSON Schema specifications can be confusing. [json-schema.org](http://json-schema.org) maintains a helpful list of [specification-links](http://json-schema.org/specification-links.html). In reverse chronological order:

 * Latest Snapshot (work in progress)
 * Draft 7
 * Draft 6
 * Draft 5
 * Draft 4
 * Draft 3
 * Drafts 0/1/2
 
 Each version updates (to varying degrees) the three parts of JSON Schema specification: Core, Validation, and Hyper-Schema.

## About
Created by Jack Wootton. Copyright 2017. Apache Licensed.
