# Zod: TypeScript-first Schema Validation Library

Zod is a TypeScript-first schema validation library that helps validate and parse data in JavaScript and TypeScript applications. It’s often used in backend validation (e.g., with Express.js), form validation in React, and API response validation.

## Why Use Zod?
- **Type-safe validation**
- **No dependencies**
- **Supports parsing** (transforming data while validating)
- **Works well with TypeScript and React Hook Form**

## Installation
```sh
npm install zod
```
###  Simple Validation
```js
import { z } from "zod";

const userSchema = z.object({
  name: z.string(),
  age: z.number().min(18), // Minimum age is 18
});

const result = userSchema.safeParse({ name: "John", age: 20 });

console.log(result.success); // true
```

###  Handling Errors
```js
const result = userSchema.safeParse({ name: "John", age: 15 });

if (!result.success) {
  console.log(result.error.format());
}
```
