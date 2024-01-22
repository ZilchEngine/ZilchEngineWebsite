 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](processstartinfo.md#processstartinfo-void)|[ApplicationName](processstartinfo.md#applicationname-zilch-eng)| | |
| |[Arguments](processstartinfo.md#arguments-zilch-engine-do)| | |
| |[RedirectStandardError](processstartinfo.md#redirectstandarderror-ze)| | |
| |[RedirectStandardInput](processstartinfo.md#redirectstandardinput-ze)| | |
| |[RedirectStandardOutput](processstartinfo.md#redirectstandardoutput-z)| | |
| |[SearchPath](processstartinfo.md#searchpath-zilch-engine-d)| | |
| |[ShowWindow](processstartinfo.md#showwindow-zilch-engine-d)| | |
| |[WorkingDirectory](processstartinfo.md#workingdirectory-zilch-en)| | |


 #  Properties


---  
 #  ApplicationName : [string](string.md)

> Name of the application to execute. No quoting of this string is necessary.
> ```TS:Nada
> var ApplicationName : String


---  
 #  Arguments : [string](string.md)

> Arguments to pass to the application.
> ```TS:Nada
> var Arguments : String


---  
 #  RedirectStandardError : [boolean](boolean.md)

> Whether or not we should redirect the Standard Error of the process for capturing.
> ```TS:Nada
> var RedirectStandardError : Boolean


---  
 #  RedirectStandardInput : [boolean](boolean.md)

> Whether or not we should redirect the Standard Input of the process for writing.
> ```TS:Nada
> var RedirectStandardInput : Boolean


---  
 #  RedirectStandardOutput : [boolean](boolean.md)

> Whether or not we should redirect the Standard Output of the process for capturing.
> ```TS:Nada
> var RedirectStandardOutput : Boolean


---  
 #  SearchPath : [boolean](boolean.md)

> Whether or not we should search the path for the application.
> ```TS:Nada
> var SearchPath : Boolean


---  
 #  ShowWindow : [boolean](boolean.md)

> Whether or not the window of the launched application should be shown.
> ```TS:Nada
> var ShowWindow : Boolean


---  
 #  WorkingDirectory : [string](string.md)

> The working directory for the process to start with. No quoting of this string is necessary.
> ```TS:Nada
> var WorkingDirectory : String


---  
 #  Methods


---  
 #  ProcessStartInfo : Void

 `constructor`

> Class used to set up parameters before launching a process.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ProcessStartInfo()
> ``` 


---  
 

 