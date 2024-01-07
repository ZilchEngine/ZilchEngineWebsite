 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Connect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/events.md#connect-void)| | | |
|[ Send](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/events.md#send-zilch-engine-documen)| | | |


 #  Properties


---  
 #  Methods


---  
 #  Connect : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |sender|[anyhandle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/anyhandle.md)| |
> |eventName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |callback|delegate()| |
> ``` lang=cpp, name=Nada
> function Connect(sender : AnyHandle, eventName : String, callback : delegate())
> ``` 


---  
 #  Send : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |sender|[anyhandle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/anyhandle.md)| |
> |eventName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[eventdata](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/eventdata.md)| |
> ``` lang=cpp, name=Nada
> function Send(sender : AnyHandle, eventName : String, event : EventData) : Integer
> ``` 


---  
 

 