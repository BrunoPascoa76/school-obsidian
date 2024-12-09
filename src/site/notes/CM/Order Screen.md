---
{"dg-publish":true,"permalink":"/cm/order-screen/"}
---

#View 
Shows current order details.

View Models: 
- [[CM/Delivery View Model\|Delivery View Model]] (shows information about current delivery, already fetched during routing) (consider changing)
- [[CM/Map View Model\|Map View Model]] (helps with managing map data)

Components:
- "See more button" (links to [[CM/Delivery Details Screen\|Delivery Details Screen]])
- [[CM/Delivery Progress Bar\|Delivery Progress Bar]]
- Map with navigation
- Basic delivery details

#TODO:
- Handle there being multiple active deliveries (more important for customer) gracefully (perhaps with a page view where you can swipe between them)
- Make proper navigation
- Unmock map location (the map is real, but the locations, apart from current are hard coded)
- Use real routing
- Make a view for customer (either don't show map at all or show only the start and end locations for the current step, perhaps?)
- Handle no current deliveries better (perhaps show some text on screen with an icon)
- #Discuss Consider hiding this route for drivers, and replace this with the [[Delivery List Screen\|Delivery List Screen]] for the customer.
- Consider changing naming from "order" to "delivery"