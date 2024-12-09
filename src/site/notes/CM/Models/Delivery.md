---
{"dg-publish":true,"permalink":"/cm/models/delivery/"}
---

#Model 
Holds information about a delivery

Fields:
- Int deliveryId
- String recipientId (refers to [[CM/Models/User\|User]])
- String senderId (refers to [[CM/Models/User\|User]])
- String driverId (refers to [[CM/Models/User\|User]])
- [[CM/Models/Parcel\|Parcel]] parcel
- String status (this is the overall status used for separating current and past deliveries. Please use "Pending", "Accepted", "In Transit" and "Delivered") (extra details are what the Steps are for)
- List\<[[CM/Models/Step\|Step]]\> steps
- Int completedSteps