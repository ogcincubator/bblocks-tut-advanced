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