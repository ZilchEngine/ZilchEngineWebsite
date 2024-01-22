 `Sound`

(NOTE) Generates audio using additive synthesis.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[AddHarmonic](additivesynthnode.md#addharmonic-void)| |[soundnode](soundnode.md)| |
|[NoteOff](additivesynthnode.md#noteoff-void)| | | |
|[NoteOn](additivesynthnode.md#noteon-void)| | | |
|[RemoveAllHarmonics](additivesynthnode.md#removeallharmonics-void)| | | |
|[StopAllNotes](additivesynthnode.md#stopallnotes-void)| | | |


 #  Properties


---  
 #  Methods


---  
 #  AddHarmonic : Void

> Adds a new harmonic to the additive synth notes. The first value is the multiplier that will be applied to the base frequency, the second is the volume of this harmonic, and the third (the AdsrEnvelope object) contains the envelope-related values.
> |Name|Type|Description|
> |---|---|---|
> |frequencyMultiplier|[real](../nada_base_types/real.md)| |
> |volume|[real](../nada_base_types/real.md)| |
> |envelope|[adsrenvelope](adsrenvelope.md)| |
> |type|[SynthWaveType](../enum_reference.md#synthwavetype)| |
> ```TS:Nada
> function AddHarmonic(frequencyMultiplier : Real, volume : Real, envelope : AdsrEnvelope, type : SynthWaveType)
> ``` 


---  
 #  NoteOff : Void

> Stops playing all current notes at the specified MIDI value.
> |Name|Type|Description|
> |---|---|---|
> |midiNote|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function NoteOff(midiNote : Real)
> ``` 


---  
 #  NoteOn : Void

> Starts playing a new note. The first parameter is the MIDI note value (range is 0 to 127), and the second is the volume modification that should be applied to this note (a value of 1.0 does not change the volume, while 0.0 would be silence).
> |Name|Type|Description|
> |---|---|---|
> |midiNote|[real](../nada_base_types/real.md)| |
> |volume|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function NoteOn(midiNote : Real, volume : Real)
> ``` 


---  
 #  RemoveAllHarmonics : Void

> Removes all current harmonics. You must add at least one harmonic before playing a note.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RemoveAllHarmonics()
> ``` 


---  
 #  StopAllNotes : Void

> Stops playing all current notes.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function StopAllNotes()
> ``` 


---  
 

 