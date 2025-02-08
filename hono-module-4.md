
## 📌 Routing
### 🔹 Hono
```ts
app.get("/user/:id", (c) => {
    const id = c.req.param("id");
    return c.json({ id, message: `User ID is ${id}` });
});
```

### 🔹 Express
```ts
app.get("/user/:id", (req, res) => {
    res.json({ id: req.params.id, message: `User ID is ${req.params.id}` });
});
```
