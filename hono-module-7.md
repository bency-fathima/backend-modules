
## 📌  Error Handling
### 🔹 Hono
```ts
app.onError((err, c) => {
    return c.json({ error: err.message }, 500);
});
```

### 🔹 Express
```ts
app.use((err, req, res, next) => {
    res.status(500).json({ error: err.message });
});
```
