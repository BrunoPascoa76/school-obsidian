---
{"dg-publish":true,"permalink":"/cm/repositories/result/"}
---

#Model 
Sealed class meant to propagate Repository's result handling to the caller.
If Result.Success, result.data will contain the output.
If Result.Error, result.exception will contain the exception

WARNING: "Result" is a name shared by many classes, including some pre-built ones. Because of that, the "suggestions" of Android Studio won't help (instead of showing an import error, the error will appear on .Success and on .Error), so you need to import Result "manually" 

Note: since all repository functions return Result\<Something\> I will omit Result when describing them. When you don't need to return anything, I usually return "true" just to avoid any troubles.