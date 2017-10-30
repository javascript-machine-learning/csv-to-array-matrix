# CSV to Matrix

CVS to Matrix parser. Reads a CSV file, outputs a arrays in array (Matrix): `npm install csv-to-matrix`

```
import math from 'mathjs';
import csvToMatrix  from 'csv-to-matrix';

csvToMatrix(pathToFile, callback, delimiter);

function callback(data) {
  const matrix = math.matrix(data);
}
```