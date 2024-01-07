 `Component` `Graphics`



(NOTE) A generated quad that addresses atlased image data for efficient frame-based animations and batched rendering.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md#sprite-void)|[ AnimationActive](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md#animationactive-zilch-eng)|[basesprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basesprite.md)| |
| |[ AnimationSpeed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md#animationspeed-zilch-engi)| | |
| |[ CurrentFrame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md#currentframe-zilch-engine)| | |
| |[ FlipX](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md#flipx-zilch-engine-docume)| | |
| |[ FlipY](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md#flipy-zilch-engine-docume)| | |
| |[ SpriteSource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md#spritesource-zilch-engine)| | |
| |[ StartFrame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md#startframe-zilch-engine-d)| | |


 #  Properties


---  
 #  AnimationActive : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If the Sprite animation should be playing on logic update, paused if false.
> ``` lang=cpp, name=Nada
> var AnimationActive : Boolean


---  
 #  AnimationSpeed : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Scalar to the amount of time passed used to advance frames of animation.
> ``` lang=cpp, name=Nada
> var AnimationSpeed : Real


---  
 #  CurrentFrame : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Index of the frame the animation is currently on.
> ``` lang=cpp, name=Nada
> var CurrentFrame : Integer


---  
 #  FlipX : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Flips the X axis of the Sprite's image (left/right).
> ``` lang=cpp, name=Nada
> var FlipX : Boolean


---  
 #  FlipY : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Flips the Y axis of the Sprite's image (top/bottom).
> ``` lang=cpp, name=Nada
> var FlipY : Boolean


---  
 #  SpriteSource : [spritesource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritesource.md)

> The resource defining one or more image sequences used for frame-based animation.
> ``` lang=cpp, name=Nada
> var SpriteSource : SpriteSource


---  
 #  StartFrame : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Index of the frame to start the animation on when the object is initialized, 0-based.
> ``` lang=cpp, name=Nada
> var StartFrame : Integer


---  
 #  Methods


---  
 #  Sprite : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Sprite()
> ``` 


---  
 

 