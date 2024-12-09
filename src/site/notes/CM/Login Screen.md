---
{"dg-publish":true,"permalink":"/cm/login-screen/"}
---

#View
Shows email and password inputs with validation. Submitting is disabled until all fields are valid.

Fields:
- Email (must contain "@")
- Password (>=8 characters)

#TODO:
- Improve email verification (research how firestore decides what is and isn't a valid email and use that)
- Stricter password requirements (Caps, numbers, non-alphanumeric characters,...)