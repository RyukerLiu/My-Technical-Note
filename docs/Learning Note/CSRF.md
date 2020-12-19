---
tags: Note
---
# CSRF

CSRF 主要發生在像 SessionBased Authentication
惡意網站透過重新導轉，透過已存在的 cookie (因為用戶未登出)達成驗證授權，進而發動惡意的 Request。

所以若是 JWT 的驗證方式，且存在 Local Storage，是可以避免 CSRF 的

reference: https://security.stackexchange.com/questions/170388/do-i-need-csrf-token-if-im-using-bearer-jwt