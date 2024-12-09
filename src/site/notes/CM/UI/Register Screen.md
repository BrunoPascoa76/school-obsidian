---
{"dg-publish":true,"permalink":"/cm/ui/register-screen/"}
---

#View 
Allows registering users. Needed fields changed based on selected role dynamically

Fields:
- Role (customer or driver) (changing this will change required fields automatically)
- Email (must contain "@")
- Password (>=8 characters)
- Confirm password (must match password)
- Full name (not empty)
- Phone number (not empty)
- Address (not empty)
- License (if driver) (not empty)
- Vehicle type (not empty)

#TODO:
- Improve email verification (research how firestore decides what is and isn't a valid email and use that)
- Stricter password requirements (Caps, numbers, non-alphanumeric characters,...)
- Better phone number verification
- use google api to store address in the Address class instead of just a string
- #Discuss make vehicle type choices limited (make it a select instead of text field)