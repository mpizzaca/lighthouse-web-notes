### Lecture Agenda
- Review, Different Data Types
- Objects

### Object Dot Notation
obj.key

### Object Squar Bracket Notation
obj['key']
- Can be used to access object with key stored in string, e.g.
```javascript
let obj = { car: 'Honda' };
let key = 'car'

obj[key] === 'Honda';
// same as
obj.car === 'Honda';
```

### `for of` vs `for in`
#### Arrays

```javascript
for (let i in array)
```
- `i` will hold the index of the current array element

```javascript
for (let elem of array)
```
- `elem` will hold the value of the current array element 


#### Objects
```javascript
for (let key in object)
```
- `key` will hold the key value of the current object element
```javascript
for (let key of object)
```
- this does not work!!!
#
### Looping through Objects
- many different ways of looping through an object
1) Most basic: for..in
```javascript
for (let key in users)
```
2) Converting the key/value pairs to an array type with Object.keys, .values, .entries
```javascript
const users = {
  1: John,
  2: Mike,
  3: Mary
}

const userKeys = Object.keys(users);
userKeys === [1, 2, 3];

const userValues = Object.values(users);
userValues === ['John', 'Mike', 'Mary'];

const userKeyValues = Object.entries(users);
userKeyValues === [
  [1, 'John'],
  [2, 'Mike'],
  [3, 'Mary']
]
```