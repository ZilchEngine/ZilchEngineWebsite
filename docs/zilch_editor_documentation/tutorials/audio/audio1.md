This lesson focuses on covering the basics of audio in Zilch Engine.

 # Learning Objectives

- Importing audio files
- Creating and playing sound cues

 # Level Setup

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename Sprite object to `Square`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent/) : [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [ SoundEmitter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundemitter.md)
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [ SimpleSound](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md)

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![AudioI](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46662.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Importing Audio

In Zilch Engine, you can play sound files by importing them as resources. There are two important resources to play audio; [Sound](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sound.md) and [SoundCue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundcue.md). By default, Zilch Engine includes both a DefaultSound resource and a DefaultSoundCue resource resources, which is what we hear when running the game. Let's experiment by adding a new sound file.

- Download the following file:
 ![Buzz](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46672.wav)
- Import it into the project by dragging and dropping the file into the `Level Window`
- In the `Import Window`
 - Set GenerateCue  to `PerSound`
 - Set GroupName  to `Buzz`
 - Press the `Import All` button



![SoundImport](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46996.gif)


Now we have added both a Sound resource and SoundCue resource resource to our project. We can verify this by looking at the `Library Window` under the respective tags.



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/88672.png)


NOTE: Zilch Engine only supports `WAV` and `OGG` audio formats, if the file you are looking to import is of a different extension, you'll need it to convert it first.

 # Sound Cue

SoundCues are resources that allow you to modify properties of a sound without altering the sound files themselves and are necessary to play any kind of audio in Zilch Engine. Let's take a look at a few of the SoundCue resource settings.



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47005.png)


| Common Sound Cue Properties |
|------|
| PlayMode enum | Whether the sound should a [Single](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#soundplaymode) time or [loop](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#soundplaymode) on completion |
| Volume  & Decibels  | How quiet or loud the sound should be played |
| Pitch  & Semitones  | How high or low pitched the sound should be played |
| VolumeVariation  | Added random volume variation within the given range when sound is played |
| PitchVariation  | Added random pitch variation within the given range when sound is played |
| Attenuator enum | The resource that defines how the sound behaves based on distance from the origin |

- In the `Library Window`
 - Under the SoundCue  tag
  - `Double-Click` Buzz 
- In the `Properties Window`
 - Set PlayMode  to `Looping`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Square object
- In the `Properties Window`
 - Under [ SimpleSound](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md)
  - Set SoundCue enum to `Buzz`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

You should now be hearing the Buzz  sound effect looping.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Attenuation

Previously, we have played sounds that remain just as loud irrespective of the emitter's position (non-positional sounds). Zilch Engine also allows us to setup sounds to be played positionally; growing louder or quieter based on the [Sound Listener](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundlistener.md)'s position, which is added by default to the `Game Camera` object.



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/88634.png)


Let's take a look on how to play positional sounds.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : 
 [Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a SoundAttenuator resource named `CustomAttenuation`
- In the `Library Window`
 - Under SoundAttenuator 
  - `Double-Click` CustomAttenuation resource
- In the `Properties Window`
 - Set StartDistance  to `10`
 - Set StopDistance  to `50`
 - Set MinAttenuatedVolume  to `0`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Square object
- In the `Properties Window`
 - Under [ SoundEmitter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundemitter.md)
  - Set Attenuator  to `CustomAttenuation`
 - Under [ SimpleSound](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md)
  - Set Positional checkBox to `true`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

If done correctly, you should notice the sound getting quieter as the Square object object falls and gets farther from the `Game Camera` which has a [SoundListener](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundlistener.md).

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Related Materials

 ## Manual
- {icon university}[[sound](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/sound.md)
- {icon university}[[soundcue](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundcue.md)
- {icon university}[[simplesound](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/simplesound.md)
- {icon university}[[soundattenuator](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundattenuator.md)
- {icon university}[[soundemitter](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundemitter.md)
- {icon university}[[soundlistener](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundlistener.md)

 ## Code Reference
 ### Classes
- [Sound](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sound.md)
- [SoundCue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundcue.md)
- [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [SoundEmitter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundemitter.md)
- [SimpleSound](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md)
- [SoundListener](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundlistener.md)
- [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)

 ### Commands
- [Create a New 2D Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
- [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#add)
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite) 

 