---
tags: Note
---

# OO多型與架構

OO影響架構最大的是：透過方法的多型，我們可以讓程式碼對於更低層的程式( Plugin 架構)的原始碼依賴中斷(透過讓多型的方法依賴於介面)。這樣一來，更低層的程式碼就可以獨立開發，以 Plugin 的方式附加。

> Python 這類的動態語言 OO 甚至連介面都省略了，完全中斷程式碼依賴性。直到 Runtime 若你定義的多型方法不如預期所定義，才直接拋出 Exception。(Duck Typing)


> Duck Typing - "If it walks like a duck and it quacks like a duck, then it must be a duck"
> https://en.wikipedia.org/wiki/Duck_typing
