
## 📌  Middleware Handling
### 🔹 Hono
```ts
const logger = async (c, next) => {
    console.log(`Request: ${c.req.method} ${c.req.path}`);
    await next();
};

app.use("*", logger);
```

### 🔹 Express
```ts
app.use((req, res, next) => {
    console.log(`Request: ${req.method} ${req.path}`);
    next();
});
```
