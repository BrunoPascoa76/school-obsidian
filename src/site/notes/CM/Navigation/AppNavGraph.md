---
{"dg-publish":true,"permalink":"/cm/navigation/app-nav-graph/"}
---

#View
Allows for navigation. All view models that are meant to be shared among screens must be initialized here to avoid problems

Routes (in [[CM/UI/Navbar\|Navbar]]):
- "home": [[CM/UI/Home Screen\|Home Screen]]
- "profile": [[CM/UI/Profile Screen\|Profile Screen]]
- "order": [[CM/UI/Order Screen\|Order Screen]] (fetches current delivery first)
- "delivery/{deliveryId}": [[CM/UI/Delivery Details Screen\|Delivery Details Screen]]

Routes (no [[CM/UI/Navbar\|Navbar]]):
- "auth": [[CM/UI/Authentication Screen\|Authentication Screen]]
- "qrCodeScanner": [[CM/UI/Qr Code Scanner Screen\|Qr Code Scanner Screen]]