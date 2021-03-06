# sigfig

[![npm version](https://img.shields.io/npm/v/sigfig)](https://npmjs.com/package/sigfig)

Retrieve the amount of significant figures in a number or round a number to a certain amount of significant figures.

## Usage

```javascript
import sigfig from 'sigfig';

sigfig('9.9', 1); // "10"
sigfig('3.10194', 4); // "3.102"
sigfig('3.10194', 7); // "3.101940"
sigfig('0.00023224', 4); // "0.0002322"

// When called without a second argument, it returns the number of
// significant figures provided in the number passed as the first argument:
sigfig('9.9'); // 2
sigfig('3.10194'); // 6
sigfig('0.00023224'); // 5
```
