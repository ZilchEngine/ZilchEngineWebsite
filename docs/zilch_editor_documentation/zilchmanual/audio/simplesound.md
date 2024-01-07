


![SimpleSound](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47916.png)


The [ SimpleSound ](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md) component, like its name suggests, is a simple way to play a sound. Choose a [SoundCue](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundcue.md), set the StartPlaying checkBox property to true, and the sound will play as soon as its object is created in an active level. 

 # Common Uses

- Looping background music 
- Sound effects that play whenever an object is created 
- An object with a single sound effect 

 # Using SimpleSound Components

SimpleSound components are dependent on the [SoundEmitter](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundemitter.md) component, so a SoundEmitter will need to be added first before the SimpleSound component. When the StartPlaying checkBox property is checked the SoundCue will be played immediately after the object is created. It can also be played by calling the `Play` method in a NadaScript. This method returns the [SoundInstance ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundinstance.md) which can then be used to further control the audio as it's playing.

 ## Positional Sound Effects

If the Positional checkBox property is checked the selected SoundCue will play through the SoundEmitter with the appropriate [SoundAttenuator ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundattenuator.md), and will be heard at that position by any [SoundListeners ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundlistener.md) in the level. In other words, if the object with the SoundEmitter is located to the left of the SoundListener on the screen, the user will hear the SoundCue more loudly from the left speaker. 

 ## Background Audio

When the Positional checkBox property is not checked the SoundCue will play directly through the [SoundSpace ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundspace.md), bypassing the SoundListeners. This is a good way to play background music or ambiance that should only be heard as long as its parent object is alive. 

---
 # Related Materials

 ## Manual

- [SoundCue ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundcue.md)
- [SoundEmitter ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundemitter.md)
- [SoundInstance ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundinstance.md)
- [SoundAttenuator ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundattenuator.md)
- [SoundListener ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundlistener.md)
- [SoundSpace ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundspace.md)

 ## Reference

- [ SimpleSound ](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md) 

 