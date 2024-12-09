---
{"dg-publish":true,"permalink":"/cm/models/step/"}
---

#Model 
Represents a stage in the delivery process

Fields:
- Address location
- String description
- Boolean isCompleted
- DateTime? completionDate (is null until isCompleted becomes true)

#TODO:
- #Discuss Add a separate "title" field and have progress bar use that instead ("title" would be a short title to appear on the progress bar, while "description" would be a more detailed explanation)