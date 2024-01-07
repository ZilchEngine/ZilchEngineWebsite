 `Component` `Engine`



(NOTE) Plays a single animation on Initialize.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ChainAnimation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simpleanimation.md#chainanimation-zilch-engi)|[ Animation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simpleanimation.md#animation-zilch-engine-do)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ CrossBlend](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simpleanimation.md#crossblend-zilch-engine-d)|[ PlayMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simpleanimation.md#playmode-zilch-engine-doc)| | |
|[ DirectBlend](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simpleanimation.md#directblend-zilch-engine)| | | |
|[ PlayIsolatedAnimation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simpleanimation.md#playisolatedanimation-ze)| | | |
|[ PlaySingle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simpleanimation.md#playsingle-zilch-engine-d)| | | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simpleanimation.md#simpleanimation-void)| | | |


 #  Properties


---  
 #  Animation : [animation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animation.md)

> Animation getter/setter.
> ``` lang=cpp, name=Nada
> var Animation : Animation


---  
 #  PlayMode : [AnimationPlayMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#animationplaymode)

> Play mode getter/setter.
> ``` lang=cpp, name=Nada
> var PlayMode : AnimationPlayMode


---  
 #  Methods


---  
 #  ChainAnimation : [animationnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animation.md)| |
> |playMode|[AnimationPlayMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Nada
> function ChainAnimation(animation : Animation, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  CrossBlend : [animationnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animation.md)| |
> |transitionTime|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |playMode|[AnimationPlayMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Nada
> function CrossBlend(animation : Animation, transitionTime : Real, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  DirectBlend : [animationnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animation.md)| |
> |transitionTime|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |playMode|[AnimationPlayMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Nada
> function DirectBlend(animation : Animation, transitionTime : Real, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  PlayIsolatedAnimation : [animationnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animation.md)| |
> |rootBone|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |playMode|[AnimationPlayMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Nada
> function PlayIsolatedAnimation(animation : Animation, rootBone : Cog, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  PlaySingle : [animationnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md)

> Play animations directly.
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animation.md)| |
> |playMode|[AnimationPlayMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Nada
> function PlaySingle(animation : Animation, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  SimpleAnimation : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SimpleAnimation()
> ``` 


---  
 

 