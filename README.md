# date-from-string
Take a string date and convert it into a date.

The little story is that while playing with dates, I stumble upon this issue: 

<img src="https://pbs.twimg.com/media/Djr2_mMX4AAbp9a.jpg" />

I tweeted my surprised, and [Matt Johnson](https://twitter.com/mj1856) who knows about dates, helped me understand basically that dates in JavaScript was a mess.

[Here's the small thread on Twitter]( https://twitter.com/sebhiticas/status/1025404401274576896)

So this helper helps create dates in a more predictable way. If you have any issues, just let me know!

## Installation 
```sh
npm install date-from-string --save
yarn add date-from-string
bower install date-from-string --save
```
## Usage
### Javascript
```javascript
var dfs = require('date-from-string');
var date = dfs.parse('2013-11-14');
```
```sh
Output should be the equivalent of new Date(2013, 10, 14); (Remember, months are 0 based index)
```
### TypeScript
```typescript
import { parse } from 'date-from-string';
console.log(parse('2013-01-01'))
```
```sh
Output should be the equivalent of new Date(2013, 1, 1); (Remember, months are 0 based index)
```
### AMD
```javascript
define(function(require,exports,module){
  var pluralise = require('date-from-string');
});
```
## Test 
```sh
npm run test
```