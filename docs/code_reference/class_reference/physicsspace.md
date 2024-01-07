 `Component` `Physics`



(NOTE) The PhysicsSpace is an "instance" of a world. This world manages and stores all of the other physical components of this world. PhysicSpaces act independently of each other.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddHierarchyPairFilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#addhierarchypairfilter-v)|[ AllowSleep](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#allowsleep-zilch-engine-d)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ AddPairFilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#addpairfilter-void)|[ CollisionTable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#collisiontable-zilch-engi)| | |
|[ CastAabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#castaabb-zilch-engine-doc)|[ Deterministic](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#deterministic-zilch-engin)| | |
|[ CastCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#castcollider-zilch-engine)|[ DynamicBroadphaseType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#dynamicbroadphasetype-ze)| | |
|[ CastFrustum](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#castfrustum-zilch-engine)|[ Mode2D](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#mode2d-zilch-engine-docum)| | |
|[ CastRay](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#castray-zilch-engine-docu)|[ PhysicsSolverConfig](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#physicssolverconfig-zero)| | |
|[ CastRayFirst](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#castrayfirst-zilch-engine)|[ StaticBroadphaseType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#staticbroadphasetype-zer)| | |
|[ CastSegment](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#castsegment-zilch-engine)|[ SubStepCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#substepcount-zilch-engine)| | |
|[ CastSphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#castsphere-zilch-engine-d)| | | |
|[ CreateJoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#createjoint-zilch-engine)| | | |
|[ DispatchWithinAabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#dispatchwithinaabb-void)| | | |
|[ DispatchWithinSphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#dispatchwithinsphere-voi)| | | |
|[ FlushPhysicsQueue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#flushphysicsqueue-void)| | | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#physicsspace-void)| | | |
|[ RemoveHierarchyPairFilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#removehierarchypairfilte)| | | |
|[ RemovePairFilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#removepairfilter-void)| | | |
|[ SweepCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#sweepcollider-zilch-engin)| | | |
|[ WhyAreTheyNotColliding](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md#whyaretheynotcolliding-z)| | | |


 #  Properties


---  
 #  AllowSleep : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if anything in the space is allowed to fall sleep.
> ``` lang=cpp, name=Nada
> var AllowSleep : Boolean


---  
 #  CollisionTable : [collisiontable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md)

> The collision table resource used to filter collisions in this space.
> ``` lang=cpp, name=Nada
> var CollisionTable : CollisionTable


---  
 #  Deterministic : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Performs extra work to help enforce determinism in the simulation.
> ``` lang=cpp, name=Nada
> var Deterministic : Boolean


---  
 #  DynamicBroadphaseType : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> What kind of broadphase is used for dynamic objects (those with RigidBodies).
> ``` lang=cpp, name=Nada
> var DynamicBroadphaseType : String


---  
 #  Mode2D : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> The default 2D mode for this space. If a RigidBody is set to InheritFromSpace then it will use this value.
> ``` lang=cpp, name=Nada
> var Mode2D : Boolean


---  
 #  PhysicsSolverConfig : [physicssolverconfig](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicssolverconfig.md)

> The resource that controls how physics solves things. Mostly related to how collision is resolved.
> ``` lang=cpp, name=Nada
> var PhysicsSolverConfig : PhysicsSolverConfig


---  
 #  StaticBroadphaseType : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> What kind of broadphase is used for static objects (those without RigidBodies).
> ``` lang=cpp, name=Nada
> var StaticBroadphaseType : String


---  
 #  SubStepCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> The number of iterations the physics space will take every frame. Used to achieve higher accuracy and increase visual results.
> ``` lang=cpp, name=Nada
> var SubStepCount : Integer


---  
 #  Methods


---  
 #  AddHierarchyPairFilter : Void

> Adds a filter to ignore collision between both hierarchies passed in. See AddPairFilter for more info.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |cog2|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function AddHierarchyPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  AddPairFilter : Void

> Filters two cogs to not resolve collisions with each other. This is a runtime only feature and will not be saved.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |cog2|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function AddPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  CastAabb : [castresultsrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that an Aabb hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)| |
> |maxCount|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |filter|[castfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Nada
> function CastAabb(aabb : Aabb, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastCollider : [castresultsrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that another collider hits using the given filter. The test collider's position can be offset to test at a different location. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |offset|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |testCollider|[collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)| |
> |filter|[castfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Nada
> function CastCollider(offset : Real3, testCollider : Collider, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastFrustum : [castresultsrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a Frustum hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |frustum|[frustum](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/frustum.md)| |
> |maxCount|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |filter|[castfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Nada
> function CastFrustum(frustum : Frustum, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastRay : [castresultsrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a ray hits. This returns up to maxCount number of objects. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md)| |
> |maxCount|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function CastRay(worldRay : Ray, maxCount : Integer) : CastResultsRange
> ``` 


---  
 #  CastRay : [castresultsrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a ray hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md)| |
> |maxCount|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |filter|[castfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Nada
> function CastRay(worldRay : Ray, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastRayFirst : [castresult](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresult.md)

> Finds the first collider that a ray hits. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md)| |
> ``` lang=cpp, name=Nada
> function CastRayFirst(worldRay : Ray) : CastResult
> ``` 


---  
 #  CastRayFirst : [castresult](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresult.md)

> Finds the first collider that a ray hits using the given filter.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md)| |
> |filter|[castfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Nada
> function CastRayFirst(worldRay : Ray, filter : CastFilter) : CastResult
> ``` 


---  
 #  CastSegment : [castresultsrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a line segment hits. This returns up to maxCount number of objects. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |segment|[segment](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/segment.md)| |
> |maxCount|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function CastSegment(segment : Segment, maxCount : Integer) : CastResultsRange
> ``` 


---  
 #  CastSegment : [castresultsrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a line segment hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |segment|[segment](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/segment.md)| |
> |maxCount|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |filter|[castfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Nada
> function CastSegment(segment : Segment, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastSphere : [castresultsrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a Sphere hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md)| |
> |maxCount|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |filter|[castfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Nada
> function CastSphere(sphere : Sphere, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CreateJoint : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Creates a joint by name (e.g. StickJoint) between two cogs. The world points of the joint are both set to worldPoint.
> |Name|Type|Description|
> |---|---|---|
> |cog0|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |cog1|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |jointName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |worldPoint|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateJoint(cog0 : Cog, cog1 : Cog, jointName : String, worldPoint : Real3) : Cog
> ``` 


---  
 #  DispatchWithinAabb : Void

> Dispatches an event to all objects within the given aabb using the provided cast filter.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)| |
> |filter|[castfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)| |
> |eventName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |toSend|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchWithinAabb(aabb : Aabb, filter : CastFilter, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinAabb : Void

> Dispatches an event to all objects within the given aabb. Uses the default cast filter.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)| |
> |eventName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |toSend|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchWithinAabb(aabb : Aabb, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinSphere : Void

> Dispatches an event to all objects within the given sphere using the provided cast filter.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md)| |
> |filter|[castfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)| |
> |eventName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |toSend|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchWithinSphere(sphere : Sphere, filter : CastFilter, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinSphere : Void

> Dispatches an event to all objects within the given sphere. Uses the default cast filter.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md)| |
> |eventName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |toSend|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchWithinSphere(sphere : Sphere, eventName : String, toSend : Event)
> ``` 


---  
 #  FlushPhysicsQueue : Void

> Forces all queued computations in physics to be updated now. Should only be used for debugging.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function FlushPhysicsQueue()
> ``` 


---  
 #  PhysicsSpace : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PhysicsSpace()
> ``` 


---  
 #  RemoveHierarchyPairFilter : Void

> Removes the filters between both hierarchies. See RemovePairFilter for more info.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |cog2|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function RemoveHierarchyPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  RemovePairFilter : Void

> Removes the filter between two cogs allowing collisions to be computed as normal.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |cog2|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function RemovePairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  SweepCollider : [sweepresultrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sweepresultrange.md)

> Performs a swept cast with a collider's shape and a given velocity. Returns a range of all objects the collider could've hit within 'dt' time.
> |Name|Type|Description|
> |---|---|---|
> |collider|[collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)| |
> |velocity|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |dt|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |filter|[castfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Nada
> function SweepCollider(collider : Collider, velocity : Real3, dt : Real, filter : CastFilter) : SweepResultRange
> ``` 


---  
 #  WhyAreTheyNotColliding : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Returns a debug string stating why physics does or doesn't think these two objects should be colliding.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |cog2|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function WhyAreTheyNotColliding(cog1 : Cog, cog2 : Cog) : String
> ``` 


---  
 

 