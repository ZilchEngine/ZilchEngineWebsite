[ SoundTags ](../../../code_reference/class_reference/soundtag.md) are resources that allow users to pause, resume, and stop a group of [SoundInstances ](soundinstance.md); control their volume, EQ, and compression; and get a list of tagged SoundInstances to change other properties in NadaScripts. 

 # Common Uses

- Controlling the volume or EQ of certain types of sounds (such as setting volume for music separately from sound effects)
- Using the `TagForDucking` and compressor properties to reduce the volume of one group of sounds when another group is playing (for instance, making sound effects quieter when dialog is playing)
- Using the compressor settings to keep a type of sound effect from getting too loud

 # Using SoundTags

SoundTags can be added to [SoundCues](soundcue.md) using [SoundTagEntries ](soundcue.md#soundtagentries). When a SoundCue is played, the resulting SoundInstance will be automatically added to all SoundTags that are on the SoundCue. Users can also add and remove SoundInstances from SoundTags in scripts at runtime. Unlike other audio objects, SoundTags exist across all Spaces, so the same SoundTag can be used for SoundInstances in different [SoundSpaces ](soundspace.md). 

 ## Volume 

The Volume  and Decibels  properties set the volume adjustment that is applied to all tagged SoundInstances. Volume  uses floating point values, while Decibels  uses the logarithmic decibel scale commonly used in audio. These properties are linked, so changing one will also change the value of the other.

Note that these volume changes will be combined with any other volume modifications applied by objects such as [SoundEmitters](soundemitter.md), SoundCues, and SoundSpaces. If a SoundCue's Volume  is set to `0.5` and it is played with a SoundTag which also has a volume of `0.5`, this effectively sets the resulting SoundInstance's volume to `0.25`.

Volume can be interpolated over time using either floating point or decibel values with the `InterpolateVolume` and `InterpolateDecibels` methods. Using these methods ensures that the volume changes are applied smoothly by the audio engine.

 ## Equalizer

If the `UseEqualizer` property is set to `true`, the EQ properties will be applied to all tagged SoundInstances. These settings control the volume of the audio at different frequency ranges. SoundTags have properties for `EQLowPassGain`, `EQBand1Gain`, `EQBand2Gain`, `EQBand3Gain`, and `EQHighPassGain`. See the [EqualizerNode ](soundnode/equalizernode.md) for explanations of how these properties work.

 ## Compressor

If the `UseCompressor` property is set to `true`, the Compressor properties will be applied to all tagged SoundInstances. A compressor reduces the volume of the sound if it goes above a specified decibel level, or threshold. SoundTags have properties for `CompressorThreshold`, `CompressorAttack`, `CompressorRelease`, `CompressorRatio`, and `CompressorKneeWidth`. See the [CompressorNode ](soundnode/compressornode.md) for explanations of how these properties work.

If the `TagForDucking` property is set to another SoundTag that tag's volume level will be used to trigger the compressor settings of this SoundTag.

 ## Nada Events

- The `AddedInstanceToTag` [ SoundEvent ](../../../code_reference/class_reference/soundevent.md) is sent when a new SoundInstance is added to the SoundTag.
- The `TagHasNoInstances` SoundEvent is sent when all SoundInstances have been removed from the SoundTag.

---
 # Resources

 ## Manual

- [SoundInstance ](soundinstance.md)
- [SoundCue ](soundcue.md)
- [SoundTagEntries ](soundcue.md#soundtagentries)
- [SoundSpace ](soundspace.md)
- [SoundEmitter ](soundemitter.md)
- [EqualizerNode ](soundnode/equalizernode.md)
- [CompressorNode ](soundnode/compressornode.md)

 ## Reference

- [ SoundTag ](../../../code_reference/class_reference/soundtag.md)
- [ SoundEvent ](../../../code_reference/class_reference/soundevent.md) 

 