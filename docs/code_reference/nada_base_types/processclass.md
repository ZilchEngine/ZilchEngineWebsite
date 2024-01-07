 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Close](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processclass.md#close-void)|[ StandardError](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processclass.md#standarderror-zilch-engin)| | |
|[ IsRunning](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processclass.md#isrunning-zilch-engine-do)|[ StandardInput](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processclass.md#standardinput-zilch-engin)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processclass.md#processclass-void)|[ StandardOutput](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processclass.md#standardoutput-zilch-engi)| | |
|[ Start](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processclass.md#start-void)| | | |
|[ Terminate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processclass.md#terminate-void)| | | |
|[ WaitForClose](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processclass.md#waitforclose-zilch-engine)| | | |


 #  Properties


---  
 #  StandardError : [filestream](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/filestream.md)

 `read-only`

> The stream where standard error is re-directed to. Null if not re-directed
> ``` lang=cpp, name=Nada
> var StandardError : FileStream


---  
 #  StandardInput : [filestream](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/filestream.md)

 `read-only`

> The stream where standard input is re-directed to. Null if not re-directed
> ``` lang=cpp, name=Nada
> var StandardInput : FileStream


---  
 #  StandardOutput : [filestream](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/filestream.md)

 `read-only`

> The stream where standard output is re-directed to. Null if not re-directed
> ``` lang=cpp, name=Nada
> var StandardOutput : FileStream


---  
 #  Methods


---  
 #  Close : Void

> Closes the wrapper around the process, does not close the process launched.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Close()
> ``` 


---  
 #  IsRunning : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Returns true if the process is still running, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IsRunning() : Boolean
> ``` 


---  
 #  ProcessClass : Void

 `constructor`

> Process class used for managing external processes and redirecting their stdio. Used to launch and monitor various external programs.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ProcessClass()
> ``` 


---  
 #  Start : Void

> Begins the execution of another process using the given parameters. 
> |Name|Type|Description|
> |---|---|---|
> |startInfo|[processstartinfo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/processstartinfo.md)| |
> ``` lang=cpp, name=Nada
> function Start(startInfo : ProcessStartInfo)
> ``` 


---  
 #  Terminate : Void

> Attempts to manually shut down the process. This is not safe for the other process or what it's handling.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Terminate()
> ``` 


---  
 #  WaitForClose : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Waits for a process to close, this will block until the process closes.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function WaitForClose() : Integer
> ``` 


---  
 

 