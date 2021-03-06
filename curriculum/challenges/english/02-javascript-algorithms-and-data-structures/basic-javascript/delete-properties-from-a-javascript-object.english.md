---
id: 56bbb991ad1ed5201cd392d3
title: Delete Properties from a JavaScript Object
challengeType: 1
---

## Description
<section id='description'>
We can also delete properties from objects like this:
<code>delete ourDog.bark;</code>
</section>

## Instructions
<section id='instructions'>
Delete the <code>"tails"</code> property from <code>myDog</code>. You may use either dot or bracket notation.
</section>

## Tests
<section id='tests'>

```yml
tests:
  - text: Delete the property <code>"tails"</code> from <code>myDog</code>.
    testString: assert(typeof myDog === "object" && myDog.tails === undefined, 'Delete the property <code>"tails"</code> from <code>myDog</code>.');
  - text: Do not modify the <code>myDog</code> setup
    testString: 'assert(code.match(/"tails": 1/g).length > 1, ''Do not modify the <code>myDog</code> setup'');'

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"],
  "bark": "bow-wow"
};

delete ourDog.bark;

// Setup
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};

// Only change code below this line.


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return z;})(myDog);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"],
  "bark": "bow-wow"
};
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};
delete myDog.tails;
```

</section>
