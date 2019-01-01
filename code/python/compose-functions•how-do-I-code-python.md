---
title: How do I code function composition in Python
---

# Sample

```
compose = lambda f,g : lambda *a,**kw : f( g( *a , **kw ) )
```

# Reduce arbitrary list of functions

```
from functools import reduce
composed = reduce( compose , (func4,func3,func2,func1) )
```

# Late-binding

```
late_binding = lambda *a,**kw : reduce(compose,(func4,func3,func2,func1))( *a , **kw ) 
```
