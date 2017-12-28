# CSV to Matrix

[![Build Status](https://travis-ci.org/javascript-machine-learning/csv-to-array-matrix.svg?branch=master)](https://travis-ci.org/javascript-machine-learning/csv-to-array-matrix)

A simple CVS to Matrix parser - reads a CSV file, outputs an arrays in array (Matrix).

## Installation

`npm install csv-to-array-matrix`

## Usage


```
import csvToMatrix  from 'csv-to-array-matrix';

csvToMatrix('./src/data.csv', callback);

function callback(data) {
  console.log(data);
}
```

Transforming into a [Matrix object with math.js](https://www.robinwieruch.de/linear-algebra-matrix-javascript/).

```
import math from 'mathjs';
import csvToMatrix  from 'csv-to-array-matrix';

csvToMatrix(pathToFile, callback);

function callback(data) {
  const matrix = math.matrix(data);
}
```

The default delimiter is ';', but you use a different one.

```
import csvToMatrix  from 'csv-to-array-matrix';

csvToMatrix('./src/data.csv', callback, ',');

function callback(data) {
  console.log(data);
}
```