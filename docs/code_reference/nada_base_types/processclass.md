 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Close](processclass.md#close-void)|[ StandardError](processclass.md#standarderror-zilch-engin)| | |
|[ IsRunning](processclass.md#isrunning-zilch-engine-do)|[ StandardInput](processclass.md#standardinput-zilch-engin)| | |
|[ Constructor](processclass.md#processclass-void)|[ StandardOutput](processclass.md#standardoutput-zilch-engi)| | |
|[ Start](processclass.md#start-void)| | | |
|[ Terminate](processclass.md#terminate-void)| | | |
|[ WaitForClose](processclass.md#waitforclose-zilch-engine)| | | |


 #  Properties


---  
 #  StandardError : [filestream](filestream.md)

 `read-only`

> The stream where standard error is re-directed to. Null if not re-directed
> ```TS:Nada
> var StandardError : FileStream


---  
 #  StandardInput : [filestream](filestream.md)

 `read-only`

> The stream where standard input is re-directed to. Null if not re-directed
> ```TS:Nada
> var StandardInput : FileStream


---  
 #  StandardOutput : [filestream](filestream.md)

 `read-only`

> The stream where standard output is re-directed to. Null if not re-directed
> ```TS:Nada
> var StandardOutput : FileStream


---  
 #  Methods


---  
 #  Close : Void

> Closes the wrapper around the process, does not close the process launched.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Close()
> ``` 


---  
 #  IsRunning : [boolean](boolean.md)

> Returns true if the process is still running, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function IsRunning() : Boolean
> ``` 


---  
 #  ProcessClass : Void

 `constructor`

> Process class used for managing external processes and redirecting their stdio. Used to launch and monitor various external programs.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ProcessClass()
> ``` 


---  
 #  Start : Void

> Begins the execution of another process using the given parameters. 
> |Name|Type|Description|
> |---|---|---|
> |startInfo|[processstartinfo](processstartinfo.md)| |
> ```TS:Nada
> function Start(startInfo : ProcessStartInfo)
> ``` 


---  
 #  Terminate : Void

> Attempts to manually shut down the process. This is not safe for the other process or what it's handling.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Terminate()
> ``` 


---  
 #  WaitForClose : [integer](integer.md)

> Waits for a process to close, this will block until the process closes.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function WaitForClose() : Integer
> ``` 


---  
 

 