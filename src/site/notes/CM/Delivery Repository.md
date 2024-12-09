---
{"dg-publish":true,"permalink":"/cm/delivery-repository/"}
---

#Model 
Handles database operations for deliveries

Data class: [[CM/Delivery\|Delivery]]
Result class: [[CM/Result\|Result]]

Functions (besides get, insert and update):
- getAllByUserIdAndStatus:
	- takes userId and either a single status and a list of status
	- filters deliveries where the user is involved (as sender, recipient or driver)
	- (if takes single status) filter deliveries where status is the same as given
	- (if takes status list) filter deliveries where status is in given list

#TODO:
- sort delivery list before returning