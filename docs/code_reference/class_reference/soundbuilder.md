 `ContentMeta`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FileLoadType](soundbuilder.md#fileloadtype-zilch-engine)|[buildercomponent](buildercomponent.md)| |
| |[ MaxVolume](soundbuilder.md#maxvolume-zilch-engine-do)| | |
| |[ Name](soundbuilder.md#name-zilch-engine-documen)| | |
| |[ Normalize](soundbuilder.md#normalize-zilch-engine-do)| | |


 #  Properties


---  
 #  FileLoadType : [AudioFileLoadType](../enum_reference.md#audiofileloadtype)

> If Streamed is selected, or if Auto is selected and the file is longer than one minute, the sound file will be streamed from disk at runtime instead of loaded into memory. Streaming files can't be played multiple times simultaneously and can't use loop tails.
> ```TS:Nada
> var FileLoadType : AudioFileLoadType


---  
 #  MaxVolume : [real](../nada_base_types/real.md)

> The volume of the sound will be altered so that the highest volume peak matches this value. All audio samples will be adjusted equally.
> ```TS:Nada
> var MaxVolume : Real


---  
 #  Name : [string](../nada_base_types/string.md)

> 
> ```TS:Nada
> var Name : String


---  
 #  Normalize : [boolean](../nada_base_types/boolean.md)

> If true, the audio will be normalized when loaded so that the highest volume peak matches the MaxVolume value.
> ```TS:Nada
> var Normalize : Boolean


---  
 #  Methods


---  
 

 