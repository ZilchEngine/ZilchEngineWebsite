 `Networking`

(NOTE) Event Bundle. Serialized event storage container.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddEvent](eventbundle.md#addevent-zilch-engine-doc)|[ GameSession](eventbundle.md#gamesession-zilch-engine)|Object| |
|[ Clear](eventbundle.md#clear-void)|[ IsEmpty](eventbundle.md#isempty-zilch-engine-docu)| | |
|[ Constructor](eventbundle.md#eventbundle-void)| | | |
|[ GetEvents](eventbundle.md#getevents-zilch-engine-do)| | | |
|[ RemoveEvent](eventbundle.md#removeevent-zilch-engine)| | | |


 #  Properties


---  
 #  GameSession : [gamesession](gamesession.md)

> Returns the game session.
> ``` lang=cpp, name=Nada
> var GameSession : GameSession


---  
 #  IsEmpty : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if the event bundle is empty (doesn't contain any events), else false.
> ``` lang=cpp, name=Nada
> var IsEmpty : Boolean


---  
 #  Methods


---  
 #  AddEvent : [boolean](../nada_base_types/boolean.md)

> Adds the event to back of the event bundle. Returns true if successful, else false (an event of that type has already been added).
> |Name|Type|Description|
> |---|---|---|
> |event|[event](event.md)| |
> ``` lang=cpp, name=Nada
> function AddEvent(event : Event) : Boolean
> ``` 


---  
 #  Clear : Void

> Clears the event bundle.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clear()
> ``` 


---  
 #  EventBundle : Void

 `constructor`

> Constructors.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function EventBundle()
> ``` 


---  
 #  EventBundle : Void

 `constructor`

> Constructors.
> |Name|Type|Description|
> |---|---|---|
> |event|[event](event.md)| |
> ``` lang=cpp, name=Nada
> function EventBundle(event : Event)
> ``` 


---  
 #  EventBundle : Void

 `constructor`

> Constructors.
> |Name|Type|Description|
> |---|---|---|
> |rhs|[eventbundle](eventbundle.md)| |
> ``` lang=cpp, name=Nada
> function EventBundle(rhs : EventBundle)
> ``` 


---  
 #  EventBundle : Void

 `constructor`

> Constructors.
> |Name|Type|Description|
> |---|---|---|
> |gameSession|[gamesession](gamesession.md)| |
> ``` lang=cpp, name=Nada
> function EventBundle(gameSession : GameSession)
> ``` 


---  
 #  EventBundle : Void

 `constructor`

> Constructors.
> |Name|Type|Description|
> |---|---|---|
> |gameSession|[gamesession](gamesession.md)| |
> |event|[event](event.md)| |
> ``` lang=cpp, name=Nada
> function EventBundle(gameSession : GameSession, event : Event)
> ``` 


---  
 #  GetEvents : [eventrange](eventrange.md)

> Returns all the events that have been added to the event bundle.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GetEvents() : EventRange
> ``` 


---  
 #  RemoveEvent : [boolean](../nada_base_types/boolean.md)

> Removes the event specified from the event bundle. Returns true if successful, else false (an event of that type has already been added).
> |Name|Type|Description|
> |---|---|---|
> |event|[event](event.md)| |
> ``` lang=cpp, name=Nada
> function RemoveEvent(event : Event) : Boolean
> ``` 


---  
 #  RemoveEvent : [boolean](../nada_base_types/boolean.md)

> Removes the event specified from the event bundle. Returns true if successful, else false (an event of that type has already been added).
> |Name|Type|Description|
> |---|---|---|
> ||[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function RemoveEvent( : String) : Boolean
> ``` 


---  
 

 