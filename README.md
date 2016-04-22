# xsd-avsc

> This project is a fork of https://github.com/elodina/xml-avro. I've changed the Converted in order to have only the XSD-->AVSC feature.

This project provides Converter to convert generic xsd to asvc files.
Avro schema is generated from xsd schema.

## Running Project
1. git clone;
2. mvn package;
3. java -jar target/xml-avro*.jar <xsdFile> {<avscFile>} // converts specified xsd to asvc files

## Schema-based converter
Usage:
```
XSD Avsc converter.
Usage: "{-d|--debug} {-b|--baseDir <baseDir>} <xsdFile> {<avscFile>}"
```

Converter has following restriction:
- complex type extensions are not supported;

## Simple converter
Usage:
```
{avro|xml} <inFile> <outFile>
```
Note: simple converter uses predefined general avro schema located at src/ly/stealth/xmlavro/simple/xml.avsc
