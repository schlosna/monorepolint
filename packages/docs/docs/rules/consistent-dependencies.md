---
title: ConsistentDependencies
---

Enforce dependency versions are consistent with workspace root.

If your root package.json has a dependency on `"somelib": "^1.0.0"` then all child projects that depend on somelib must also have that version listed.

### Example

```javascript
import { ConsistentDependencies } from "monorepolint/rules";
export default {
  rules: [
    new ConsistentDependencies({}),
  ],
};
```

[rule source](https://github.com/monorepolint/monorepolint/blob/master/packages/rules/src/consistentDependencies.ts)
