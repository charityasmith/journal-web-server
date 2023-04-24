# Notes on ES6

ECMAScript = ESx. ES3...ES^, ESNext

## Variables
```javascript
let a = 'Hello World!';
const b = {};
```

## Functions
```javascript
function a() {} // 'this' defined whenever function is defined

const b = () => {}; // 'this' defined on onw scope
```

## Arrays & Objects
```javascript
const arr = [1,2,3,4,5];
const [first, ... otherNumbers] = arr;

const obj = { name: 'bob'};
const {name} = obj;
```

## Promises
```javascript
const p = new Promise((resolve, reject) => {
    if(err) {
        reject(false)
    }
    resolve(true);
});

// old method
p.then(val => console.log(value)).then().catch(err);

// new method
async function a() {
    return await p;
}
```