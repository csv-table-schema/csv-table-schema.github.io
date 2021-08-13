Simple CSV Schema is a pragmatic approach for defining [CSV](https://datatracker.ietf.org/doc/html/rfc4180) schemas. Simple CSV Schema provides a CSV schema description via JSON.

Main features:

+ Easy schema definiton via JSON which can be validated against the [Simple CSV Meta Schema](https://github.com/simple-csv-schema/simple-csv-schema.spec/blob/main/src/simple-csv-schema.json).
+ Dedicated to the CSV format.
+ Supports the following data types: string, enum, enum-set, bool, int, float, date, time, date-time, json and xml.
+ Supports CSV tables with ordered and unordered columns.
+ Supports CSV tables with or without header line.

## Examples

The following examples are available:

* [Sample 01a: List of Students](https://github.com/simple-csv-schema/simple-csv-schema.spec/samples/sample01a.scsv.json)
* [Sample 01b: List of Courses](https://github.com/simple-csv-schema/simple-csv-schema.spec/samples/sample01b.scsv.json)
* [Sample 01c: List of Subjects](https://github.com/simple-csv-schema/simple-csv-schema.spec/samples/sample01b.scsv.json)

## Why yet another CSV schema definition?

Unlike JSON or XML there is no well established schema definition language for CSV. But we are of course not the first ones with a proposal:

+ The [CSV Schema Language](https://digital-preservation.github.io/csv-schema/csv-schema-1.2.html) is a language for defining and validating CSV data. It uses its [own domain language](http://digital-preservation.github.io/csv-schema/csv-schema-1.2.html#ebnf) for describing the schema. 
+ The [Table Schema](https://specs.frictionlessdata.io/table-schema/) is a format to declare a schema for tabular data (CSV is just one example). The schema is designed to be expressible in JSON.

Both approaches are well thought but sadly didn't suit our needs.

Simple CSV Schema is an alternative schema description which is heavily inspired by both existing schema languages.

## What's missing?

A data schema has two purposes:

+ Semantical documentation of the data structure
+ The possibility to validate real data against the data schema.

The documentation part is done. What's still missing is a reference validator.
