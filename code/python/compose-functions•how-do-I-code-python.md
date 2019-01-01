---
title: How do I code function composition in Python
---

# Sample

```
compose = lambda f,g : lambda *a,**kw : f( g( *a , **kw ) )
```
