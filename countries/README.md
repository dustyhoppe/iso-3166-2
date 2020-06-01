# ISO-3166-2

This repo contains a collection of JSON files with ISO-3166-2 country and subdivision codes sourced from Wikipedia.


## Contents

The [countries.json](countries.json) file contains the ISO-3166-2 codes for each country.

An country entry in the `countries.json` is a json object with the following structure:

```json
{
  "code": "country code:string",
  "name": "country name:string"
}
```

For each of those countries, there is a file with the name `{country-code}.json` that contains the collection of subdivisions within that country and their ISO-3166-2 codes. 

For example: the file for Mexico is named [mx.json](mx.json).

A subdivision entry in the country specific file is a json object with the following structure:

```json
{
  "code": "subdivision code:string",
  "name": "subdivision name:string",
  "category": "an optional category that subdivision belongs to:string"
}
```