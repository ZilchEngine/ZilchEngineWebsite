 `Component` `Physics`



(NOTE) Allows a user to send out collision events that do not originate from the physics system. This includes determining when to send start/persisted/end events. This is primarily intended for use with a swept character controller where you never actually come into contact with objects. The objects you would have hit can be added to this so that the same logic can be used for swept and non-swept collision.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[AddCollision](customcollisioneventtracker.md#addcollision-void)| |[component](component.md)| |
|[Constructor](customcollisioneventtracker.md#customcollisioneventtrac)| | | |
|[SendEvents](customcollisioneventtracker.md#sendevents-void)| | | |


 #  Properties


---  
 #  Methods


---  
 #  AddCollision : Void

> Add a collision for this frame between ourself and the passed in collider.
> |Name|Type|Description|
> |---|---|---|
> |otherCollider|[collider](collider.md)| |
> |worldPoint|[real3](../nada_base_types/real3.md)| |
> |worldNormalTowardsOther|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function AddCollision(otherCollider : Collider, worldPoint : Real3, worldNormalTowardsOther : Real3)
> ``` 


---  
 #  CustomCollisionEventTracker : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CustomCollisionEventTracker()
> ``` 


---  
 #  SendEvents : Void

> Send out all of the events that have been queued up. This includes determining what should be started/persisted/ended events. These events are sent with the prefix that is passed in, e.g. if you pass in 'Collision' then CollisionStarted, CollisionPersisted, and CollisionEnded will be the event names.
> |Name|Type|Description|
> |---|---|---|
> |eventPrefix|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function SendEvents(eventPrefix : String)
> ``` 


---  
 

 