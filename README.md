# Grafter Test Transformations

## Datasets
- celica
- people

## Usage

As for now, we've got two different transformations, so the pipeline name will always be one of the names in the above list. Files containing data will also start it's name with the name of the above datasets. The same will apply to the transformations functions itself.

Below, you will find clear examples of usage, having to replace 'PROJECTNAME' with one of the datasets names ;)

### Leiningen

`lein grafter run graftertransformations.pipeline/convert-PROJECTNAME-to-data ./data/PROJECTNAME-data.csv ./output/PROJECTNAME-data.csv`

`lein grafter run graftertransformations.pipeline/convert-PROJECTNAME-data-to-graph ./data/PROJECTNAME-data.csv ./output/PROJECTNAME-data.rdf`

## TODO

- When a cell in the csv file is empty, do not create a triple, because it's useless

## Travis Tests Results
[![Build Status](https://travis-ci.org/xaabi6/Grafter-Transformations.svg?branch=master)](https://travis-ci.org/xaabi6/Grafter-Transformations)
