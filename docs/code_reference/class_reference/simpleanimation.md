 `Component` `Engine`



(NOTE) Plays a single animation on Initialize.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ChainAnimation](simpleanimation.md#chainanimation-zilch-engi)|[Animation](simpleanimation.md#animation-zilch-engine-do)|[component](component.md)| |
|[CrossBlend](simpleanimation.md#crossblend-zilch-engine-d)|[PlayMode](simpleanimation.md#playmode-zilch-engine-doc)| | |
|[DirectBlend](simpleanimation.md#directblend-zilch-engine)| | | |
|[PlayIsolatedAnimation](simpleanimation.md#playisolatedanimation-ze)| | | |
|[PlaySingle](simpleanimation.md#playsingle-zilch-engine-d)| | | |
|[Constructor](simpleanimation.md#simpleanimation-void)| | | |


 #  Properties


---  
 #  Animation : [animation](animation.md)

> Animation getter/setter.
> ```TS:Nada
> var Animation : Animation


---  
 #  PlayMode : [AnimationPlayMode](../enum_reference.md#animationplaymode)

> Play mode getter/setter.
> ```TS:Nada
> var PlayMode : AnimationPlayMode


---  
 #  Methods


---  
 #  ChainAnimation : [animationnode](animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](animation.md)| |
> |playMode|[AnimationPlayMode](../enum_reference.md#animationplaymode)| |
> ```TS:Nada
> function ChainAnimation(animation : Animation, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  CrossBlend : [animationnode](animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](animation.md)| |
> |transitionTime|[real](../nada_base_types/real.md)| |
> |playMode|[AnimationPlayMode](../enum_reference.md#animationplaymode)| |
> ```TS:Nada
> function CrossBlend(animation : Animation, transitionTime : Real, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  DirectBlend : [animationnode](animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](animation.md)| |
> |transitionTime|[real](../nada_base_types/real.md)| |
> |playMode|[AnimationPlayMode](../enum_reference.md#animationplaymode)| |
> ```TS:Nada
> function DirectBlend(animation : Animation, transitionTime : Real, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  PlayIsolatedAnimation : [animationnode](animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](animation.md)| |
> |rootBone|[cog](cog.md)| |
> |playMode|[AnimationPlayMode](../enum_reference.md#animationplaymode)| |
> ```TS:Nada
> function PlayIsolatedAnimation(animation : Animation, rootBone : Cog, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  PlaySingle : [animationnode](animationnode.md)

> Play animations directly.
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](animation.md)| |
> |playMode|[AnimationPlayMode](../enum_reference.md#animationplaymode)| |
> ```TS:Nada
> function PlaySingle(animation : Animation, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  SimpleAnimation : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function SimpleAnimation()
> ``` 


---  
 

 