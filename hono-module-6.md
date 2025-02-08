

## 📌  Handling POST Requests
### 🔹 Hono
```ts
app.post("/data", async (c) => {
    const body = await c.req.json();
    return c.json({ success: true, data: body });
});
```

### 🔹 Express
```ts
app.use(express.json());

app.post("/data", (req, res) => {
    res.json({ success: true, data: req.body });
});
```
