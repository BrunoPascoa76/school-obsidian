---
{"dg-publish":true,"permalink":"/cm/app-nav-graph/"}
---

#View
Allows for navigation. All view models that are meant to be shared among screens must be initialized here to avoid problems

Routes (in [[CM/Navbar\|Navbar]]):
- "home": [[CM/Home Screen\|Home Screen]]
- "profile": [[CM/Profile Screen\|Profile Screen]]
- "order": [[CM/Order Screen\|Order Screen]] (fetches current delivery first)
- "delivery/{deliveryId}": [[CM/Delivery Details Screen\|Delivery Details Screen]]

Routes (no [[CM/Navbar\|Navbar]]):
- "auth": [[CM/Authentication Screen\|Authentication Screen]]
- "qrCodeScanner": [[CM/Qr Code Scanner Screen\|Qr Code Scanner Screen]]