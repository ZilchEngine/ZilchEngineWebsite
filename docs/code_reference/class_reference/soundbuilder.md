 `ContentMeta`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FileLoadType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundbuilder.md#fileloadtype-zilch-engine)|[buildercomponent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/buildercomponent.md)| |
| |[ MaxVolume](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundbuilder.md#maxvolume-zilch-engine-do)| | |
| |[ Name](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundbuilder.md#name-zilch-engine-documen)| | |
| |[ Normalize](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundbuilder.md#normalize-zilch-engine-do)| | |


 #  Properties


---  
 #  FileLoadType : [AudioFileLoadType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#audiofileloadtype)

> If Streamed is selected, or if Auto is selected and the file is longer than one minute, the sound file will be streamed from disk at runtime instead of loaded into memory. Streaming files can't be played multiple times simultaneously and can't use loop tails.
> ``` lang=cpp, name=Nada
> var FileLoadType : AudioFileLoadType


---  
 #  MaxVolume : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume of the sound will be altered so that the highest volume peak matches this value. All audio samples will be adjusted equally.
> ``` lang=cpp, name=Nada
> var MaxVolume : Real


---  
 #  Name : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> 
> ``` lang=cpp, name=Nada
> var Name : String


---  
 #  Normalize : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If true, the audio will be normalized when loaded so that the highest volume peak matches the MaxVolume value.
> ``` lang=cpp, name=Nada
> var Normalize : Boolean


---  
 #  Methods


---  
 

 