 `Engine`

(NOTE) Base action class.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Cancel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/action.md#cancel-void)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/action.md#active-zilch-engine-docum)|[referencecountedeventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/referencecountedeventobject.md)|[actiondelay](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actiondelay.md)|
| |[ Completed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/action.md#completed-zilch-engine-do)| |[actionset](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actionset.md)|
| |[ Started](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/action.md#started-zilch-engine-docu)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> The action is queued and not stared or running.
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  Completed : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> The action ran until it completed.
> ``` lang=cpp, name=Nada
> var Completed : Boolean


---  
 #  Started : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Has the action started?
> ``` lang=cpp, name=Nada
> var Started : Boolean


---  
 #  Methods


---  
 #  Cancel : Void

> Cancel the action and all child actions.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Cancel()
> ``` 


---  
 

 