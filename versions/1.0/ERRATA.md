# Errata for Workflow Description Language version 1.0 specification

## WDL_1_0.E001

in [Struct Assignment from Object Literal](./SPEC.md#struct-assignment-from-object-literal)

```wdl

Person a = {"name": "John","age": 30}

```

should be 

```wdl

Person a = object {name: "John", age: 30}

```

(the original text shows a [map literal](./SPEC.md#map-literals) rather than an [object literal](./SPEC.md#object-literals)).

## WDL_1_0.E002

Description built-in function [read_json()](./SPEC.md#mixed-read_jsonstringfile) says in one place that the argument should be a
TSV file -- in fact it should be a JSON file.

## WDL_1_0.E003

In illustration of [computing task inputs](./SPEC.md#task-inputs), an intermediate variable is incorrectly described as being an input when
the point of the illustration is that that it is *not* an input.


