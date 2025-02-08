
###  Optional and Default Values
```js
const schema = z.object({
  username: z.string(),
  isAdmin: z.boolean().default(false),
});

console.log(schema.parse({ username: "Alice" }));
// Output: { username: 'Alice', isAdmin: false }
```

###  Arrays and Nested Objects
```js
const userSchema = z.object({
  name: z.string(),
  emails: z.array(z.string().email()), // Array of valid email strings
});

console.log(userSchema.parse({ name: "Sam", emails: ["sam@email.com"] }));
```

###  Using Zod with Express.js
```js
import express from "express";
import { z } from "zod";

const app = express();
app.use(express.json());

const userSchema = z.object({
  name: z.string(),
  age: z.number().min(18),
});

app.post("/users", (req, res) => {
  const parsed = userSchema.safeParse(req.body);

  if (!parsed.success) {
    return res.status(400).json(parsed.error.format());
  }

  res.json({ message: "User data is valid!", data: parsed.data });
});

app.listen(3000, () => console.log("Server running on port 3000"));
```
