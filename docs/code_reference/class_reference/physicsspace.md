 `Component` `Physics`



(NOTE) The PhysicsSpace is an "instance" of a world. This world manages and stores all of the other physical components of this world. PhysicSpaces act independently of each other.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddHierarchyPairFilter](physicsspace.md#addhierarchypairfilter-v)|[ AllowSleep](physicsspace.md#allowsleep-zilch-engine-d)|[component](component.md)| |
|[ AddPairFilter](physicsspace.md#addpairfilter-void)|[ CollisionTable](physicsspace.md#collisiontable-zilch-engi)| | |
|[ CastAabb](physicsspace.md#castaabb-zilch-engine-doc)|[ Deterministic](physicsspace.md#deterministic-zilch-engin)| | |
|[ CastCollider](physicsspace.md#castcollider-zilch-engine)|[ DynamicBroadphaseType](physicsspace.md#dynamicbroadphasetype-ze)| | |
|[ CastFrustum](physicsspace.md#castfrustum-zilch-engine)|[ Mode2D](physicsspace.md#mode2d-zilch-engine-docum)| | |
|[ CastRay](physicsspace.md#castray-zilch-engine-docu)|[ PhysicsSolverConfig](physicsspace.md#physicssolverconfig-zero)| | |
|[ CastRayFirst](physicsspace.md#castrayfirst-zilch-engine)|[ StaticBroadphaseType](physicsspace.md#staticbroadphasetype-zer)| | |
|[ CastSegment](physicsspace.md#castsegment-zilch-engine)|[ SubStepCount](physicsspace.md#substepcount-zilch-engine)| | |
|[ CastSphere](physicsspace.md#castsphere-zilch-engine-d)| | | |
|[ CreateJoint](physicsspace.md#createjoint-zilch-engine)| | | |
|[ DispatchWithinAabb](physicsspace.md#dispatchwithinaabb-void)| | | |
|[ DispatchWithinSphere](physicsspace.md#dispatchwithinsphere-voi)| | | |
|[ FlushPhysicsQueue](physicsspace.md#flushphysicsqueue-void)| | | |
|[ Constructor](physicsspace.md#physicsspace-void)| | | |
|[ RemoveHierarchyPairFilter](physicsspace.md#removehierarchypairfilte)| | | |
|[ RemovePairFilter](physicsspace.md#removepairfilter-void)| | | |
|[ SweepCollider](physicsspace.md#sweepcollider-zilch-engin)| | | |
|[ WhyAreTheyNotColliding](physicsspace.md#whyaretheynotcolliding-z)| | | |


 #  Properties


---  
 #  AllowSleep : [boolean](../nada_base_types/boolean.md)

> Determines if anything in the space is allowed to fall sleep.
> ```TS:Nada
> var AllowSleep : Boolean


---  
 #  CollisionTable : [collisiontable](collisiontable.md)

> The collision table resource used to filter collisions in this space.
> ```TS:Nada
> var CollisionTable : CollisionTable


---  
 #  Deterministic : [boolean](../nada_base_types/boolean.md)

> Performs extra work to help enforce determinism in the simulation.
> ```TS:Nada
> var Deterministic : Boolean


---  
 #  DynamicBroadphaseType : [string](../nada_base_types/string.md)

> What kind of broadphase is used for dynamic objects (those with RigidBodies).
> ```TS:Nada
> var DynamicBroadphaseType : String


---  
 #  Mode2D : [boolean](../nada_base_types/boolean.md)

> The default 2D mode for this space. If a RigidBody is set to InheritFromSpace then it will use this value.
> ```TS:Nada
> var Mode2D : Boolean


---  
 #  PhysicsSolverConfig : [physicssolverconfig](physicssolverconfig.md)

> The resource that controls how physics solves things. Mostly related to how collision is resolved.
> ```TS:Nada
> var PhysicsSolverConfig : PhysicsSolverConfig


---  
 #  StaticBroadphaseType : [string](../nada_base_types/string.md)

> What kind of broadphase is used for static objects (those without RigidBodies).
> ```TS:Nada
> var StaticBroadphaseType : String


---  
 #  SubStepCount : [integer](../nada_base_types/integer.md)

> The number of iterations the physics space will take every frame. Used to achieve higher accuracy and increase visual results.
> ```TS:Nada
> var SubStepCount : Integer


---  
 #  Methods


---  
 #  AddHierarchyPairFilter : Void

> Adds a filter to ignore collision between both hierarchies passed in. See AddPairFilter for more info.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](cog.md)| |
> |cog2|[cog](cog.md)| |
> ```TS:Nada
> function AddHierarchyPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  AddPairFilter : Void

> Filters two cogs to not resolve collisions with each other. This is a runtime only feature and will not be saved.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](cog.md)| |
> |cog2|[cog](cog.md)| |
> ```TS:Nada
> function AddPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  CastAabb : [castresultsrange](castresultsrange.md)

> Finds all colliders in the space that an Aabb hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](aabb.md)| |
> |maxCount|[integer](../nada_base_types/integer.md)| |
> |filter|[castfilter](castfilter.md)| |
> ```TS:Nada
> function CastAabb(aabb : Aabb, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastCollider : [castresultsrange](castresultsrange.md)

> Finds all colliders in the space that another collider hits using the given filter. The test collider's position can be offset to test at a different location. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |offset|[real3](../nada_base_types/real3.md)| |
> |testCollider|[collider](collider.md)| |
> |filter|[castfilter](castfilter.md)| |
> ```TS:Nada
> function CastCollider(offset : Real3, testCollider : Collider, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastFrustum : [castresultsrange](castresultsrange.md)

> Finds all colliders in the space that a Frustum hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |frustum|[frustum](frustum.md)| |
> |maxCount|[integer](../nada_base_types/integer.md)| |
> |filter|[castfilter](castfilter.md)| |
> ```TS:Nada
> function CastFrustum(frustum : Frustum, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastRay : [castresultsrange](castresultsrange.md)

> Finds all colliders in the space that a ray hits. This returns up to maxCount number of objects. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](ray.md)| |
> |maxCount|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function CastRay(worldRay : Ray, maxCount : Integer) : CastResultsRange
> ``` 


---  
 #  CastRay : [castresultsrange](castresultsrange.md)

> Finds all colliders in the space that a ray hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](ray.md)| |
> |maxCount|[integer](../nada_base_types/integer.md)| |
> |filter|[castfilter](castfilter.md)| |
> ```TS:Nada
> function CastRay(worldRay : Ray, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastRayFirst : [castresult](castresult.md)

> Finds the first collider that a ray hits. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](ray.md)| |
> ```TS:Nada
> function CastRayFirst(worldRay : Ray) : CastResult
> ``` 


---  
 #  CastRayFirst : [castresult](castresult.md)

> Finds the first collider that a ray hits using the given filter.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](ray.md)| |
> |filter|[castfilter](castfilter.md)| |
> ```TS:Nada
> function CastRayFirst(worldRay : Ray, filter : CastFilter) : CastResult
> ``` 


---  
 #  CastSegment : [castresultsrange](castresultsrange.md)

> Finds all colliders in the space that a line segment hits. This returns up to maxCount number of objects. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |segment|[segment](segment.md)| |
> |maxCount|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function CastSegment(segment : Segment, maxCount : Integer) : CastResultsRange
> ``` 


---  
 #  CastSegment : [castresultsrange](castresultsrange.md)

> Finds all colliders in the space that a line segment hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |segment|[segment](segment.md)| |
> |maxCount|[integer](../nada_base_types/integer.md)| |
> |filter|[castfilter](castfilter.md)| |
> ```TS:Nada
> function CastSegment(segment : Segment, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastSphere : [castresultsrange](castresultsrange.md)

> Finds all colliders in the space that a Sphere hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](sphere.md)| |
> |maxCount|[integer](../nada_base_types/integer.md)| |
> |filter|[castfilter](castfilter.md)| |
> ```TS:Nada
> function CastSphere(sphere : Sphere, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CreateJoint : [cog](cog.md)

> Creates a joint by name (e.g. StickJoint) between two cogs. The world points of the joint are both set to worldPoint.
> |Name|Type|Description|
> |---|---|---|
> |cog0|[cog](cog.md)| |
> |cog1|[cog](cog.md)| |
> |jointName|[string](../nada_base_types/string.md)| |
> |worldPoint|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function CreateJoint(cog0 : Cog, cog1 : Cog, jointName : String, worldPoint : Real3) : Cog
> ``` 


---  
 #  DispatchWithinAabb : Void

> Dispatches an event to all objects within the given aabb using the provided cast filter.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](aabb.md)| |
> |filter|[castfilter](castfilter.md)| |
> |eventName|[string](../nada_base_types/string.md)| |
> |toSend|[event](event.md)| |
> ```TS:Nada
> function DispatchWithinAabb(aabb : Aabb, filter : CastFilter, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinAabb : Void

> Dispatches an event to all objects within the given aabb. Uses the default cast filter.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](aabb.md)| |
> |eventName|[string](../nada_base_types/string.md)| |
> |toSend|[event](event.md)| |
> ```TS:Nada
> function DispatchWithinAabb(aabb : Aabb, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinSphere : Void

> Dispatches an event to all objects within the given sphere using the provided cast filter.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](sphere.md)| |
> |filter|[castfilter](castfilter.md)| |
> |eventName|[string](../nada_base_types/string.md)| |
> |toSend|[event](event.md)| |
> ```TS:Nada
> function DispatchWithinSphere(sphere : Sphere, filter : CastFilter, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinSphere : Void

> Dispatches an event to all objects within the given sphere. Uses the default cast filter.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](sphere.md)| |
> |eventName|[string](../nada_base_types/string.md)| |
> |toSend|[event](event.md)| |
> ```TS:Nada
> function DispatchWithinSphere(sphere : Sphere, eventName : String, toSend : Event)
> ``` 


---  
 #  FlushPhysicsQueue : Void

> Forces all queued computations in physics to be updated now. Should only be used for debugging.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function FlushPhysicsQueue()
> ``` 


---  
 #  PhysicsSpace : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PhysicsSpace()
> ``` 


---  
 #  RemoveHierarchyPairFilter : Void

> Removes the filters between both hierarchies. See RemovePairFilter for more info.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](cog.md)| |
> |cog2|[cog](cog.md)| |
> ```TS:Nada
> function RemoveHierarchyPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  RemovePairFilter : Void

> Removes the filter between two cogs allowing collisions to be computed as normal.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](cog.md)| |
> |cog2|[cog](cog.md)| |
> ```TS:Nada
> function RemovePairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  SweepCollider : [sweepresultrange](sweepresultrange.md)

> Performs a swept cast with a collider's shape and a given velocity. Returns a range of all objects the collider could've hit within 'dt' time.
> |Name|Type|Description|
> |---|---|---|
> |collider|[collider](collider.md)| |
> |velocity|[real3](../nada_base_types/real3.md)| |
> |dt|[real](../nada_base_types/real.md)| |
> |filter|[castfilter](castfilter.md)| |
> ```TS:Nada
> function SweepCollider(collider : Collider, velocity : Real3, dt : Real, filter : CastFilter) : SweepResultRange
> ``` 


---  
 #  WhyAreTheyNotColliding : [string](../nada_base_types/string.md)

> Returns a debug string stating why physics does or doesn't think these two objects should be colliding.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](cog.md)| |
> |cog2|[cog](cog.md)| |
> ```TS:Nada
> function WhyAreTheyNotColliding(cog1 : Cog, cog2 : Cog) : String
> ``` 


---  
 

 