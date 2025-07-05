---
icon: square-code
---

# Architecture

The `SystemDirectory` and `SystemFile` classes utilize getters and setters for most properties. This is to abolish the need for getter and setter functions (such as `getPath()` and `setPath()`). All getters and setters are synchronous, so no `Promise`s are used.

```typescript
// Instead of...
await file.setPath("./example/path");
// ...@raynecloudy/fs does this:
file.path = "./example/path";
```
