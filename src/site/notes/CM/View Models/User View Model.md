---
{"dg-publish":true,"permalink":"/cm/view-models/user-view-model/"}
---

#Controller
Does operations involving the user and authentication

Repositories:
- [[CM/Repositories/User Repository\|User Repository]] holds the actual user "profile"

Other technologies:
- Firebase auth (does the authentication as a way to get user's uid)

Functions:
- login
	- takes email and password
	- gets user uid from Firebase auth then uses it to fetch user table
- register
	- takes email, password, full name, phone number, address and role (overload exists that also takes license and vehicle type)
	- registers the user
	- if successful, also creates database entry
- logout
	- signs out from firebase
	- sets state to null
- fetch user table (private)
	- takes uid
	- fetches user table from uid
- create user table (private)
	- takes user
	- created database entry
- update
	- takes user
	- (if anything changed) updates user table
	- (if email changes) update email in firebase auth (due to Firebase policy, the user needs to verify email change via email-sent link before the verification is completed)

#TODO 
- update address to use actual Address class
- deal with any back-end logic Address selection might required (if any)
- rewrite exceptions to use custom messages