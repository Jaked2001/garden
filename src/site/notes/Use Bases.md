---
{"dg-publish":true,"permalink":"/use-bases/"}
---

# [[Use Bases\|Use Bases]]


Show overdue if date is over today

```js
if(due_date < now() && status != "Done", "Overdue", "")

// Use the one below with my configuration
if(Data > now(), Data.relative(), if(Stato != "🟢 Fatto", "OVERDUE", "Done"))
```

