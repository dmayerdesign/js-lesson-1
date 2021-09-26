# Types

Code does things with data — that's 100% of what it does. Data is what we call the information that our code is supposed to interpret, transform, analyze, do math with, etc. When we write our code (we call this "compile time" or "design time"), we have to make lots of educated guesses about what that data is going to be when the program is running ("run time"), so that we can make guarantees — even if they're not exact ones — about what the program will do in the real world.

Every language implements the concept of types a little bit differently. Here's how JavaScript does it.

In JavaScript, there are a few basic types, called primitives:

- `boolean`
- `number`
- `string`
- `undefined`

Every other type in JavaScript is something called a `class`, which is sort of just another word for "type". As the name implies, classes are meant to define a list of properties so that our code can create "instances" of it, each instance having different values for those properties. So, if you had a class called `Dog`, you might give it properties like `color` or `weight`, and you might create multiple instances of `Dog` in your code (perhaps based on some raw data you read from a dog database). Each instance you create will represent a chunk of data that your code cares about. The same is true for primitives — sometimes the data isn't as complex as a dog, and is represented by something simple like a number or a "true or false".

The difference between classes and primitives is really just that classes contain multiple data, where primitives contain just one datum. The properties of `Dog`, like `color` and `weight`, might themselves be primitive data types (color might be a string, and weight might be a number). Something like `weight` might alternatively be represented by a class itself, maybe one called `Weight` that has properties like `amount` and `unitOfMeasurement`.

Here are some JavaScript examples of how types work in the language.

```js

const iAmANumber = 2;
// Initializing the variable iAmANumber to 2 sets its data type to "number".
// This is what JavaScript would call the "literal" way of writing a number.
// (Every primitive has its own class — number has Number, string has String, etc.
// We consider those the "non-literal" version, and in practice they're almost never used.)

console.log(typeof iAmANumber);
// JavaScript has a special keyword called typeof.
// Writing typeof followed by some variable will return ("evaluate to") the name of its type when run.
// This line would write the string "number" to the console.

```


