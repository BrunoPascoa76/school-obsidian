---
{"dg-publish":true,"permalink":"/cm/delivery-progress-bar/"}
---

#View 
Display's a delivery progress.

View models:
- [[CM/Delivery View Model\|Delivery View Model]] (has the needed data)

Features:
- Each step is represented as a circle
- Progress between steps is represented as a circle
- Completed steps are highlighted
- Bars between completed steps are fully filled
- Bars between uncompleted steps are empty
- Bar between last completed step and the next step is filled based on distance (%) already driven.
- Properly handles nulls (hides itself)

#TODO:
- Unmock progress once we get real-time db working (currently hard coded at 50%)
- Verify if it handles 2 steps being at the same location properly (for example, if "accepted" and "driver left for pickup" are separate steps, how does it display it?)
- #Discuss on clicking the circle it could show (either in a popup/dialog/modal or a separate page) more details for the step (location, completion time,detailed description)
- Allow drivers to conclude current step (if it's the last one, it will redirect to qr code instead)
- Allow drivers to add an extra step in-between this one and the next (this is important because packages are often transfered between sorting centers because of logistics and we do NOT want the user to see the progress decrease) (as an example, my package went through 4 sorting centers in Lisbon alone because of Christmas)