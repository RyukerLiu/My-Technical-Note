---
tags: 坑, Learning Note
---

# Aggregate vs Annotate Sum

Annotate Count
``` python
X.values('a', 'b').distinct().annotate(c_count=Count('c', distinct=True))
```

由於Group_by(values) a 和 b 然後在 Annotate Count, distinct by c, 所以每個 Group 裡面的 c 是不會重複的 (Group內 c 不會重複, 但在 Group 之間 c 有可能重複)


Aggregate Count
``` python 
X.aggregate(c_count=Count('c', distinct=True))
```

而 Aggregate Count, distinct by c, 以整體 X 來看, 其中之 c 不會重複)

所以當你用 Annotate 的 Distinct c_count 加總, 是會大於 Aggreate 的 Distinct c_count 的 (因為 Group 之間會有重複的受眾)