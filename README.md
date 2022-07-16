# Modern ( ES6+ ) Javscript Snippets for Sublime Text 4

Modern Javascript Snippets for use with Javascript, Typescript and JSX files.

### Credits
I have refactored the snippets created by [tunnckoCore](https://github.com/tunnckoCore) to be used for Sublime Text 4. 

The original snippets were created for Atom & VSCode and can be found [here](https://github.com/tunnckoCore/modern-javascript-snippets).


### Install
To use snippets, you can clone/fork the repo into the following folder or any subfolder of this directory.

```
C:\Users\%username%\AppData\Roaming\Sublime Text\Packages\User
```

### Snippet Table of Contents
- [Snippets](#snippets)
  * [assert](#assert)
  * [async](#async)
  * [classes](#classes)
  * [console](#console)
  * [control-flow](#control-flow)
  * [declarations](#declarations)
  * [events](#events)
  * [functions](#functions)
  * [iterables](#iterables)
  * [json](#json)
  * [loops](#loops)
  * [misc](#misc)
  * [modules-commonjs](#modules-commonjs)
  * [modules-es2015](#modules-es2015)
  * [objects](#objects)
  * [returns](#returns)
  * [testing](#testing)
  * [timers](#timers)
  * [types](#types)



### Snippet
## Snippets

### assert
> All [assert](./assert) snippets

#### `ase⇥` assert.strictEqual

```js
${1:assert}.strictEqual(${2:actual}, ${3:expected})${0}
```

#### `asn⇥` assert.notStrictEqual

```js
${1:assert}.notStrictEqual(${2:actual}, ${3:expected})${0}
```

#### `asd⇥` assert.deepStrictEqual

```js
${1:assert}.deepStrictEqual(${2:actual}, ${3:expected})${0}
```

#### `asdn⇥` assert.notDeepStrictEqual

```js
${1:assert}.notDeepStrictEqual(${2:actual}, ${3:expected})${0}
```

#### `asi⇥` assert.ifError

```js
${1:assert}.ifError(${2:err})${0}
```

#### `ast⇥` assert.throws

```js
${1:assert}.throws(${2:actual}, ${3:expected})${0}
```

**[back to top](#readme)**

### async
> All [async](./async) snippets

#### `cb⇥` Node callback

```js
(err, ${1:value}) => {
  ${0}
}
```

#### `p⇥` Promise constructor

```js
new Promise((resolve${1:, reject}) => {
  ${0}
})
```

#### `then⇥` Promise.then

```js
${1:promise}.then((${2:value}) => {${0}})
```

#### `.then⇥` chain then

```js
.then((${1:value}) => {${0}})
```

#### `catch⇥` Promise.catch

```js
${1:promise}.catch((${2:err}) => {${0}})
```

#### `.catch⇥` chain catch

```js
.catch((${1:err}) => {${0}})
```

#### `aw⇥` await

```js
await ${0}
```

**[back to top](#readme)**

### classes
> All [classes](./classes) snippets

#### `cs⇥` class

```js
class ${1:ClassName} {
  constructor (${2:args}) {
    ${3}
  }
}
```

#### `csx⇥` class extends

```js
class ${1:ClassName} extends ${2:BaseClass} {
  constructor (${3:args}) {
    super(${3:args})
    ${4}
  }
}
```

#### `csm⇥` class method

```js
${1:name} (${2:args}) {
  ${3}
}
```

#### `csi⇥` es5 singleton class

```js
function ${1:ClassName} (${2:args}) {
  if (!(this instanceof ${1:ClassName})) {
    return new ${1:ClassName}(${2:args})
  }
  ${3}
}
```

#### `csf⇥` es5 function class

```js
function ${1:ClassName} (${2:args}) {
  ${3}
}
```

**[back to top](#readme)**

### console
> All [console](./console) snippets

#### `cl⇥` console.log

```js
console.log(${0})
```

#### `ce⇥` console.error

```js
console.error(${0})
```

#### `cw⇥` console.warn

```js
console.warn(${0})
```

#### `cd⇥` console.dir

```js
console.dir(${0})
```

**[back to top](#readme)**

### control-flow
> All [control-flow](./control-flow) snippets

#### `if⇥` if statement

```js
if (${1:condition}) {
  ${2}
}
```

#### `el⇥` else statement

```js
else {
  ${1}
}
```

#### `ife⇥` if/else statement

```js
if (${1:condition}) {
  ${2}
} else {
  ${3}
}
```

#### `ei⇥` else if statement

```js
else if (${1:condition}) {
  ${2}
}
```

#### `tc⇥` try/catch

```js
try {
  ${1}
} catch (${2:err}) {
  ${3}
}
```

#### `tf⇥` try/finally

```js
try {
  ${1}
} finally {
  ${2}
}
```

#### `tcf⇥` try/catch/finally

```js
try {
  ${1}
} catch (${2:err}) {
  ${3}
} finally {
  ${4}
}
```

**[back to top](#readme)**

### declarations
> All [declarations](./declarations) snippets

#### `v⇥` var statement

```js
var ${1:name}
```

#### `v=⇥` var assignment

```js
var ${1:name} = ${2:value}
```

#### `l⇥` let statement

```js
let ${1:name}
```

#### `l=⇥` let assignment

```js
let ${1:name} = ${2:value}
```
#### `ly⇥` let yielded

```js
let ${1:name} = yield ${2:value}
```

#### `la⇥` let awaited

```js
let ${1:name} = await ${2:value}
```

#### `c⇥` const statement

```js
const ${1:name}
```

#### `c=⇥` const assignment

```js
const ${1:name} = ${2:value}
```

#### `cy⇥` const yielded

```js
const ${1:name} = yield ${2:value}
```

#### `ca⇥` const awaited

```js
const ${1:name} = await ${2:value}
```

#### `co⇥` const object

```js
const ${1:name} = {
  ${2}
}
```

#### `ca⇥` const array

```js
const ${1:name} = [
  ${2}
]
```

**[back to top](#readme)**

### events
> All [events](./events) snippets

#### `on⇥` on event handler

```js
${1:emitter}.on('${2:event}', ${3:args})
```

#### `.on⇥` chain .on

```js
.on('${1:event}', ${2:handler})
```

#### `once⇥` once event handler

```js
${1:emitter}.once('${2:event}', ${3:args})
```

#### `.once⇥` chain .once

```js
.once('${1:event}', ${2:handler})
```

#### `emit⇥` emit event

```js
${1:emitter}.emit('${2:event}', ${3:args})
```

#### `.emit⇥` chain .emit

```js
.emit('${1:event}', ${2:args})
```

**[back to top](#readme)**

### functions
> All [functions](./function) snippets

#### `f⇥` anonymous function

```js
function (${1:args}) {${0}}
```

#### `fn⇥` named function

```js
function ${1:name} (${2:args}) {${0}}
```

#### `asf⇥` async anonymous function

```js
async function (${1:args}) {${0}}
```

#### `asfn⇥` async named function

```js
async function ${1:name} (${2:args}) {${0}}
```

#### `af⇥` arrow function

```js
(${1:args}) => ${2:statement}
```

#### `afn⇥` arrow fn with body

```js
(${1:args}) => {${0}}
```

#### `gf⇥` generator

```js
function * (${1:args}) {${0}}
```

#### `gfn⇥` named generator

```js
function * ${1:name} (${2:args}) {${0}}
```

#### `iife⇥` immediately-invoked function expression

```js
;(function (${1:args}) {
  ${0}
})(${2})
```

#### `fa⇥` function apply

```js
${1:fn}.apply(${2:this}, ${3:args})
```

#### `fc⇥` function call

```js
${1:fn}.call(${2:this}, ${3:args})
```

#### `fb⇥` function bind

```js
${1:fn}.bind(${2:this}, ${3:args})
```

**[back to top](#readme)**

### iterables
> All [iterables](./iterables) snippets

#### `fe⇥` forEach loop

```js
${1:iterable}.forEach(${2:iterator})
```

#### `.fe⇥` chain forEach

```js
.forEach(${1:iterator})
```

#### `map⇥` map

```js
${1:iterable}.map(${2:iterator})
```

#### `.map⇥` chain map

```js
.map(${1:iterator})
```

#### `reduce⇥` reduce

```js
${1:iterable}.reduce((${2:previous}, ${3:current}) => {
  ${0}
}${4:, initial})
```

#### `.reduce⇥` chain reduce

```js
.reduce((${1:previous}, ${2:current}) => {
  ${0}
}${3:, initial})
```

#### `filter⇥` filter

```js
${1:iterable}.filter(${2:iterator})
```

#### `.filter⇥` chain filter

```js
.filter(${1:iterator})
```

#### `find⇥` find

```js
${1:iterable}.find(${2:iterator})
```

#### `.find⇥` chain find

```js
.find(${1:iterator})
```

#### `every⇥` every

```js
${1:iterable}.every(${2:iterator})
```

#### `.every⇥` chain every

```js
.every(${1:iterator})
```

#### `some⇥` some

```js
${1:iterable}.some(${2:iterator})
```

#### `.some⇥` chain some

```js
.some(${1:iterator})
```

**[back to top](#readme)**

### json
> All [json](./json) snippets

#### `;⇥` JSON key/value pair

```js
"${1:key}": "${2:value}"
```

#### `;a⇥` JSON key/array pair

```js
"${1:key}": ["${2:values}"]
```

#### `;o⇥` JSON key/object pair

```js
"${1:key}": {"${2:values}"}
```

#### `;t⇥` JSON true

```js
"${1:key}": true
```

#### `;f⇥` JSON false

```js
"${1:key}": false
```

#### `js⇥` JSON.stringify()

```js
JSON.stringify($0)
```

#### `jp⇥` JSON.parse()

```js
JSON.parse($0)
```


**[back to top](#readme)**

### loops
> All [loops](./loops) snippets

#### `fl⇥` for loop

```js
for (let ${1:i} = 0; ${1:i} < ${2:iterable}${3:.length}; ${1:i}++) {
  ${4}
}
```

#### `fi⇥` for in loop

```js
for (let ${1:key} in ${2:source}) {
  if (${2:source}.hasOwnProperty(${1:key})) {
    ${3}
  }
}
```

#### `fo⇥` for of loop

```js
for (let ${1:key} of ${2:source}) {
  ${3}
}
```

#### `wl⇥` while loop

```js
while (${1:condition}) {
  ${2}
}
```

**[back to top](#readme)**

### modules
> All [modules](./modules) snippets

#### `ex⇥` module export

```js
export ${1:member}
```

#### `exd⇥` module default export

```js
export default ${1:member}
```

#### `im⇥` import module

```js
import ${2:name} from '${1:pkg}'${3}
```

#### `ima⇥` import module as

```js
import ${2:*} as ${3:name} from '${1:pkg}'${4}
```

#### `imd⇥` import module destructured

```js
import { $2 } from '${1:pkg}'${3}
```

**[back to top](#readme)**

### objects
> All [objects](./objects) snippets

#### `kv⇥` key/value pair

```js
${1:key}: ${2:'value'}
```

#### `proto⇥` prototype method

```js
${1:ClassName}.prototype.${2:key} = ${3:value}
```

#### `.proto⇥` chain prototype method

```js
.prototype.${2:key} = ${3:value}
```

#### `ok⇥` Object.keys

```js
Object.keys(${1:obj})${0}
```

#### `ov⇥` Object.values

```js
Object.values(${1:obj})${0}
```

**[back to top](#readme)**

### returns
> All [returns](././atom/returns.cson) snippets

#### `r⇥` return

```js
return ${0}
```

#### `rth⇥` return this

```js
return this
```

#### `rn⇥` return null

```js
return null
```

#### `rt⇥` return true

```js
return true
```

#### `rf⇥` return false

```js
return false
```

#### `r0⇥` return 0

```js
return 0
```

#### `r-1⇥` return -1

```js
return -1
```

#### `rp⇥` return promise

```js
return new Promise((resolve${1:, reject}) => {
  ${0}
})
```

**[back to top](#readme)**


### timers
> All [timers](././atom/timers.cson) snippets

#### `st⇥` setTimeout

```js
setTimeout(() => {
  ${0}
}, ${1:delay})
```

#### `si⇥` setInterval

```js
setInterval(() => {
  ${0}
}, ${1:delay})
```

#### `sim⇥` setImmediate

```js
setImmediate(() => {
  ${0}
})
```

**[back to top](#readme)**