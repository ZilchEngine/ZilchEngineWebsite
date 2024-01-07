 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processstartinfo.md#processstartinfo-void)|[ ApplicationName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processstartinfo.md#applicationname-zilch-eng)| | |
| |[ Arguments](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processstartinfo.md#arguments-zilch-engine-do)| | |
| |[ RedirectStandardError](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processstartinfo.md#redirectstandarderror-ze)| | |
| |[ RedirectStandardInput](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processstartinfo.md#redirectstandardinput-ze)| | |
| |[ RedirectStandardOutput](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processstartinfo.md#redirectstandardoutput-z)| | |
| |[ SearchPath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processstartinfo.md#searchpath-zilch-engine-d)| | |
| |[ ShowWindow](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processstartinfo.md#showwindow-zilch-engine-d)| | |
| |[ WorkingDirectory](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processstartinfo.md#workingdirectory-zilch-en)| | |


 #  Properties


---  
 #  ApplicationName : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Name of the application to execute. No quoting of this string is necessary.
> ``` lang=cpp, name=Nada
> var ApplicationName : String


---  
 #  Arguments : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Arguments to pass to the application.
> ``` lang=cpp, name=Nada
> var Arguments : String


---  
 #  RedirectStandardError : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not we should redirect the Standard Error of the process for capturing.
> ``` lang=cpp, name=Nada
> var RedirectStandardError : Boolean


---  
 #  RedirectStandardInput : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not we should redirect the Standard Input of the process for writing.
> ``` lang=cpp, name=Nada
> var RedirectStandardInput : Boolean


---  
 #  RedirectStandardOutput : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not we should redirect the Standard Output of the process for capturing.
> ``` lang=cpp, name=Nada
> var RedirectStandardOutput : Boolean


---  
 #  SearchPath : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not we should search the path for the application.
> ``` lang=cpp, name=Nada
> var SearchPath : Boolean


---  
 #  ShowWindow : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not the window of the launched application should be shown.
> ``` lang=cpp, name=Nada
> var ShowWindow : Boolean


---  
 #  WorkingDirectory : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> The working directory for the process to start with. No quoting of this string is necessary.
> ``` lang=cpp, name=Nada
> var WorkingDirectory : String


---  
 #  Methods


---  
 #  ProcessStartInfo : Void

 `constructor`

> Class used to set up parameters before launching a process.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ProcessStartInfo()
> ``` 


---  
 

 