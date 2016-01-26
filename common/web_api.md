# Web API Desiging Rules

## Design

Use [Swagger 2.0]() to design / define API. And provide JSON/YAML format document for it. You can use [Swagger Editor](editor.swagger.io) to design APIs.

## Versioning

Use [Semantic versioning](http://semver.org/). Major version will be changed when you need to do braking changes. Minor/Patch version up might keep backward compativility.

Include version number in URL like `http://api.example.com/v1/users`. use "v" + major version. Never include minor version because minor version up need to ensure backward compativility.

## 
