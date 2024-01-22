 `Component` `Graphics`



(NOTE) A generated quad that addresses atlased image data for efficient frame-based animations and batched rendering.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](sprite.md#sprite-void)|[AnimationActive](sprite.md#animationactive-zilch-eng)|[basesprite](basesprite.md)| |
| |[AnimationSpeed](sprite.md#animationspeed-zilch-engi)| | |
| |[CurrentFrame](sprite.md#currentframe-zilch-engine)| | |
| |[FlipX](sprite.md#flipx-zilch-engine-docume)| | |
| |[FlipY](sprite.md#flipy-zilch-engine-docume)| | |
| |[SpriteSource](sprite.md#spritesource-zilch-engine)| | |
| |[StartFrame](sprite.md#startframe-zilch-engine-d)| | |


 #  Properties


---  
 #  AnimationActive : [boolean](../nada_base_types/boolean.md)

> If the Sprite animation should be playing on logic update, paused if false.
> ```TS:Nada
> var AnimationActive : Boolean


---  
 #  AnimationSpeed : [real](../nada_base_types/real.md)

> Scalar to the amount of time passed used to advance frames of animation.
> ```TS:Nada
> var AnimationSpeed : Real


---  
 #  CurrentFrame : [integer](../nada_base_types/integer.md)

> Index of the frame the animation is currently on.
> ```TS:Nada
> var CurrentFrame : Integer


---  
 #  FlipX : [boolean](../nada_base_types/boolean.md)

> Flips the X axis of the Sprite's image (left/right).
> ```TS:Nada
> var FlipX : Boolean


---  
 #  FlipY : [boolean](../nada_base_types/boolean.md)

> Flips the Y axis of the Sprite's image (top/bottom).
> ```TS:Nada
> var FlipY : Boolean


---  
 #  SpriteSource : [spritesource](spritesource.md)

> The resource defining one or more image sequences used for frame-based animation.
> ```TS:Nada
> var SpriteSource : SpriteSource


---  
 #  StartFrame : [integer](../nada_base_types/integer.md)

> Index of the frame to start the animation on when the object is initialized, 0-based.
> ```TS:Nada
> var StartFrame : Integer


---  
 #  Methods


---  
 #  Sprite : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Sprite()
> ``` 


---  
 

 