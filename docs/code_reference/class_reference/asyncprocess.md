 `Engine`

(NOTE) A process class that asynchronously reads from standard output and standard error and sends out partial read events. Additionally, the full buffer can be stored for each stream. This makes it possible to read the output of a process in a single-threaded context without having to block on output.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Close](asyncprocess.md#close-void)|[StandardError](asyncprocess.md#standarderror-zilch-engin)|[referencecountedeventobject](referencecountedeventobject.md)| |
|[Create](asyncprocess.md#create-zilch-engine-docum)|[StandardInput](asyncprocess.md#standardinput-zilch-engin)| | |
|[IsRunning](asyncprocess.md#isrunning-zilch-engine-do)|[StandardOutput](asyncprocess.md#standardoutput-zilch-engi)| | |
|[Start](asyncprocess.md#start-zilch-engine-docume)|[StoreStandardErrorData](asyncprocess.md#storestandarderrordata-z)| | |
|[Terminate](asyncprocess.md#terminate-void)|[StoreStandardOutputData](asyncprocess.md#storestandardoutputdata)| | |
|[WaitForClose](asyncprocess.md#waitforclose-zilch-engine)| | | |


 #  Properties


---  
 #  StandardError : [string](../nada_base_types/string.md)

 `read-only`

> The cached total results from standard error. Will be empty if StoreStandardErrorData is false.
> ```TS:Nada
> var StandardError : String


---  
 #  StandardInput : [filestream](../nada_base_types/filestream.md)

> 
> ```TS:Nada
> var StandardInput : FileStream


---  
 #  StandardOutput : [string](../nada_base_types/string.md)

 `read-only`

> The cached total results from standard output. Will be empty if StoreStandardOutputData is false.
> ```TS:Nada
> var StandardOutput : String


---  
 #  StoreStandardErrorData : [boolean](../nada_base_types/boolean.md)

> Should the results from standard error be accumulated and stored? If a lot of data is output it may be good to turn this off and use the partial data callback events instead.
> ```TS:Nada
> var StoreStandardErrorData : Boolean


---  
 #  StoreStandardOutputData : [boolean](../nada_base_types/boolean.md)

> Should the results from standard output be accumulated and stored? If a lot of data is output it may be good to turn this off and use the partial data callback events instead.
> ```TS:Nada
> var StoreStandardOutputData : Boolean


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
 #  Create : [asyncprocess](asyncprocess.md)

 `static`

> Construct a new process. This does not start the process.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Create() : AsyncProcess
> ``` 


---  
 #  IsRunning : [boolean](../nada_base_types/boolean.md)

> Returns true if the process is still running, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function IsRunning() : Boolean
> ``` 


---  
 #  Start : [boolean](../nada_base_types/boolean.md)

> Begins the execution of another process using the given parameters. Throws an exception if the process cannot be started.
> |Name|Type|Description|
> |---|---|---|
> |startInfo|[processstartinfo](../nada_base_types/processstartinfo.md)| |
> ```TS:Nada
> function Start(startInfo : ProcessStartInfo) : Boolean
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
 #  WaitForClose : [integer](../nada_base_types/integer.md)

> Waits for a process to close, this will block until the process closes.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function WaitForClose() : Integer
> ``` 


---  
 #  WaitForClose : [integer](../nada_base_types/integer.md)

> Waits for a process to close up to a given number of milliseconds. This can take up to 3 * milliseconds due to waiting for the output streams to close.
> |Name|Type|Description|
> |---|---|---|
> |milliseconds|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function WaitForClose(milliseconds : Integer) : Integer
> ``` 


---  
 

 