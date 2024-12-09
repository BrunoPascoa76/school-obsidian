---
{"dg-publish":true,"permalink":"/cm/ui/authentication-screen/"}
---

#View
Allows for authentication. Appears only if user is logged out.

View Models: [[CM/View Models/User View Model\|User View Model]] for the authentication (also reacts to changes in order to redirect to home screen as soon as user is not null)

Has tabs for:
- [[CM/UI/Login Screen\|Login Screen]]
- [[CM/UI/Register Screen\|Register Screen]]

#TODO:
- use custom error messages instead of the ones Firestore returns
- improve validation
- if I ever change the main screen from "home" to something else, also change here