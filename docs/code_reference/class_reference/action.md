 `Engine`

(NOTE) Base action class.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Cancel](action.md#cancel-void)|[ Active](action.md#active-zilch-engine-docum)|[referencecountedeventobject](referencecountedeventobject.md)|[actiondelay](actiondelay.md)|
| |[ Completed](action.md#completed-zilch-engine-do)| |[actionset](actionset.md)|
| |[ Started](action.md#started-zilch-engine-docu)| | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

 `read-only`

> The action is queued and not stared or running.
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  Completed : [boolean](../nada_base_types/boolean.md)

 `read-only`

> The action ran until it completed.
> ``` lang=cpp, name=Nada
> var Completed : Boolean


---  
 #  Started : [boolean](../nada_base_types/boolean.md)

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
 

 