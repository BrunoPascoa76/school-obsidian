---
{"dg-publish":true,"permalink":"/cm/delivery-view-model/"}
---

#Controller
Does operations regarding deliveries

Repositories:
- [[CM/Delivery Repository\|Delivery Repository]]
- [[CM/User Repository\|User Repository]] (for fetching related users)

States:
- state (delivery)
- error message
- driver, sender and recipient (related to delivery)

Features:
- fetch delivery
	- receives deliveryId
	- returns delivery with said id
- fetch current delivery
	- received user
	- fetches all current ("Pending", "Accepted" or "In Transit") deliveries that the user is involved in (if user is not null) and saves first one (does not give error is user has no deliveries)
- submit Qr Code
	- received qr code as string
	- compares it with id and, if it matches, increments step
- increment Delivery Status
	- increments completed steps
- get Related users
	- retrieves users associated to the delivery

#TODO:
- #Discuss in fetch delivery, consider only allowing to fetch deliveries in which the user is involved (is either the sender, recipient or driver)
- allow to show multiple current deliveries (since this would be a List\<Delivery\> and not a simple Delivery, may use a separate view model)
- sort current deliveries somehow before choosing the first one (wanted to do earliest first, but that will require an extra field, which shouldn't be too hard)
- when incrementing steps, forgot to mark current as done
- In qr code submission, consider just completing the delivery all-together
- #Discuss in get related users, is it an "all or nothing scenario" (if 1 user fails fetching, should we fail completely, should we fail completely or should we keep it null (screens that use users should already be prepared to handles nulls because of the driver))