Display JSON data.

Display the key, value, and data type of the value.

Data types used are boolean, number, string, array, and object.

Example display of single item:
```
  amount [number]: 1952.82
```

For arrays, use the index as the key.

Child elements should be indented beneath parent.

Objects and arrays should have a control for expanding / collapsing. 

Example:
```
 tags [array]: {{EXPAND/COLLAPSE CONTROL}}
   0 [string]: "culpa"
   ...
 nested [object]: {{EXPAND/COLLAPSE CONTROL}}
   child1 [string]: "Dolore mollit"
   ...
```

Arrays can also contain objects, and vice-versa:
```
 arrayOfObjects [array]: {{EXPAND/COLLAPSE CONTROL}}
   0 [object]: {{EXAND/COLLAPSE CONTROL}}
     child1 [string]: "Dolore mollit"
     ...
   1 [object]: {{EXAND/COLLAPSE CONTROL}}
     child1 [string]: "Lorem ipsum"
     ...
 objectWithArray [object] {{EXAND/COLLAPSE CONTROL}}
   child1 [array]: {{EXAND/COLLAPSE CONTROL}}
     0 [string]: "culpa"
     ...
   child2 [array]: {{EXAND/COLLAPSE CONTROL}}
     0 [string]: "Dolore molliti"
```

Bonus: Include a control at the top to expand/collapse the entire structure.


Use the following sample JSON:  [sample.json](sample.json)

In your application, fetch the data from [https://fsteger.github.io/tmp-pki-interview/sample.json](https://fsteger.github.io/pki-interview-json-viewer/sample.json)

