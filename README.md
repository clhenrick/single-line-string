# Single Line String
Converts multiline ES6 template strings to a single line & removes extra whitespace.
Requires a javascript environment that supports [template strings](#)

## Usage
ES6

```
import sls from 'single-line-string';

var name = 'June';
const hello = sls`
  Hey,
        hello,
  how
    are
              you
  ${name}?
`

console.log(hello); // outputs: "Hey, hello, how are you June?"
```

or via Common JS

```
var sls = require('single-line-string');
var name = 'June';
var hello = sls`
  Hey,
        hello,
  how
    are
              you
  ${name}?
`;

console.log(hello); // outputs: "Hey, hello, how are you June?"
```

## Build
`npm install && npm run build`

## Test
`node test/test.js`

## Credits
code credit: https://muffinresearch.co.uk/removing-leading-whitespace-in-es6-template-strings/
