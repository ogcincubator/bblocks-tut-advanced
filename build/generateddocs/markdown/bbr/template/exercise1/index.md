
# Compo (Model)

`ogc.bbr.template.exercise1` *v0.1*

Refactor into ontology + rules, schema and binding profile

[*Status*](http://www.opengis.net/def/status): Under development

## Description

## Exercise 4

An example of the end result is available [here](bblocks://ogc.bbr.tutorial.exercise1_completed)

Goal: Refactor a schema + ontology binding to allow re-use of ontology with multiple schemas

Note this illustrates how to use examples to test rules fail when expected. This is a critical capability for complex systems.

### Steps
- uncomment import from schema.yaml
- uncomment line #11 in rules.shacl and examine the additional profile constraint (B<5))
- run build
- run viewer

- view validation results on "about tab"
- move `examples/*-fail` to `tests`
- run build
- run viewer
- view validation results at [Validation Report](validation) or [build-local/...](/register/build-local/tests/bbr/template/exercise3/_report.json)
## Examples

### Valid under new rule
#### json
```json
{
  "a": "mynamespace:aThing",
  "b": 6,
  "c": 1
}


```

#### jsonld
```jsonld
{
  "@context": [
    {
      "mynamespace": "http://example.org/ns1/"
    },
    {}
  ],
  "a": "mynamespace:aThing",
  "b": 6,
  "c": 1
}
```

#### ttl
```ttl


```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-tut-advanced/undefined/build/annotated/bbr/template/exercise1/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-tut-advanced/undefined/build/annotated/bbr/template/exercise1/schema.yaml)

## Sources

* [Sample source document](https://example.com/sources/1)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-tut-advanced](https://github.com/ogcincubator/bblocks-tut-advanced)
* Path: `_sources/exercise1`

