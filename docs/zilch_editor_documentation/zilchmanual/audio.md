
 # [Sound ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/sound.md)

A Sound resource is created for every imported audio file. Sounds can be attached to any number of SoundCues, allowing the user to play the same sound multiple ways while only storing the file once.

 # [SoundCue ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundcue.md)

SoundCues are a fundamental part of playing audio in the Zilch Engine, allowing the user to modify various properties without affecting the original Sound resource.

 # [SimpleSound ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/simplesound.md)

The SimpleSound component, like its name suggests, is a simple way to play a sound, requiring only a SoundEmitter component and a SoundCue.

 # [SoundAttenuator ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundattenuator.md)

The SoundAttenuator resource controls how a sound played through a SoundEmitter on an object decreases in volume as the object gets further away from a SoundListener.

 # [SoundEmitter ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundemitter.md)

The SoundEmitter component handles the 3D positioning of sounds in a level. 

 # [SoundInstance ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundinstance.md)

SoundInstances are created at runtime whenever a SoundCue is played, and can then be controlled by the user in scripts.

 # [SoundListener ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundlistener.md)

The SoundListener component �hears� all positional audio in a SoundSpace.

 # [SoundSpace ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundspace.md)

The SoundSpace keeps sounds separate from other Spaces and allows the user to control overall settings for all audio in the SoundSpace.

 # [SoundTag ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundtag.md)

SoundTags are resources that allow users to pause, resume, and stop a group of SoundInstances; control their volume, EQ, and compression; and get a list of tagged SoundInstances to change other properties in NadaScripts.

 # [Volume Meter ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/volume_meter.md)

The Volume Meter tool allows the user to monitor and change the audio system volume. 

 # [SoundNode ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundnode.md)

SoundNodes are the underlying objects which create and modify all audio in the Zilch Engine. Many types of SoundNodes can only be created and added to the node graph in NadaScripts.

 # [SoundNode Graph ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundnode_graph.md)

The SoundNode Graph tool displays the connections between all SoundNodes that are currently attached to the output of a SoundSpace. 

 # [MIDI ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/midi.md)

If a MIDI device is connected when the Zilch Engine starts up it will listen for messages from that device and send corresponding MidiEvents. 

 # [AudioSettings ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/audiosettings.md)

The AudioSettings component can be added to Zilch Engine's project settings to control project-wide audio settings. 

 