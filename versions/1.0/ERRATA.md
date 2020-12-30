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
