---
tags: Note
---


# DNS Domain and Subdomain

如果買了 Domain Name 後, 就擁有了整個 Namespace, 包含 subdomain

只是要在 DNS Server 上做對應的設定

像是用 CNAME 把 subdomain 映射到其他的 domain name

或是用 A Record 把 subdomain 指到某個 IP Address


## Domain and Subdomain IP

subdomain 是可以指到與 parent domain 不同的 IP 的

有的 DNS Server 會提供 wildcard, 所以才會有好像不管哪個 subdomain 都指到同一個 IP 的感覺