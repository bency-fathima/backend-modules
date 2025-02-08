
## 📌  Authentication & JWT
### 🔹 Hono
```ts
import { jwt } from "hono/jwt";

app.use("/secure/*", jwt({ secret: "supersecret" }));

app.get("/secure/data", (c) => c.text("Protected data!"));
```

### 🔹 Express
```ts
import jwt from "jsonwebtoken";

app.use("/secure/*", (req, res, next) => {
    const token = req.headers.authorization?.split(" ")[1];
    if (!token) return res.status(401).json({ error: "Unauthorized" });

    jwt.verify(token, "supersecret", (err, user) => {
        if (err) return res.status(403).json({ error: "Forbidden" });
        req.user = user;
        next();
    });
});

app.get("/secure/data", (req, res) => res.send("Protected data!"));
```
