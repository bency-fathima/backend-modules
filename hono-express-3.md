
## 📌  Basic API Setup
### 🔹 Hono
```ts
import { Hono } from "hono";

const app = new Hono();

app.get("/", (c) => c.text("Hello from Hono!"));

export default app;
```

### 🔹 Express
```ts
import express from "express";

const app = express();

app.get("/", (req, res) => {
    res.send("Hello from Express!");
});

app.listen(3000, () => console.log("Server running on port 3000"));
```
