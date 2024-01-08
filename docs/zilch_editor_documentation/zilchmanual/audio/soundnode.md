SoundNodes are the objects which create and modify all audio in the Zilch Engine. If you are new to SoundNodes and the SoundNode graph, be sure to read the overview page first.

- [SoundNode Overview ](soundnode/soudnode_overview.md)
- [SoundNode Graph Tool ](soundnode_graph.md)

 # Generating Audio

 ## [GeneratedWaveNode ](soundnode/generatedwavenode.md)

Creates audio at a specified pitch using generated audio waves.

 ## [AdditiveSynthNode ](soundnode/additivesynthnode.md)

Plays notes at specified pitches using additive synthesis.

 ## [CustomAudioNode ](soundnode/customaudionode.md)

Allows the user to pass buffers of audio data directly to the audio engine for output.

 # Volume and Pitch Modifications

 ## [VolumeNode ](soundnode/volumenode.md)

Changes the volume of the audio provided by its inputs.

 ## [Panning Node ](soundnode/panningnode.md)

Changes the volume of the left and right channels of the audio provided by its inputs separately.

 ## [PitchNode ](soundnode/pitchnode.md)

Changes the pitch of the audio provided by its inputs.

 ## [EqualizerNode ](soundnode/equalizernode.md)

Changes the volume of the audio provided by its inputs in certain frequency ranges.

 ## [CompressorNode ](soundnode/compressornode.md)

Applies a compressor filter to the audio provided by its inputs.

 ## [ExpanderNode ](soundnode/expandernode.md)

Applies an expander filter to the audio provided by its inputs.

 # Audio Effect Filters

 ## [ReverbNode ](soundnode/reverbnode.md)

Applies a simple reverb filter to the audio provided by its inputs.

 ## [LowPassNode ](soundnode/lowpassnode.md)

Applies a low pass filter to the audio provided by its inputs (removes high frequencies).

 ## [HighPassNode ](soundnode/highpassnode.md)

Applies a high pass filter to the audio provided by its inputs (removes low frequencies).

 ## [BandPassNode ](soundnode/bandpassnode.md)

Applies a band pass filter to the audio provided by its inputs (removes frequencies higher and lower than the band).

 ## [DelayNode ](soundnode/delaynode.md)

Applies a delay filter to the audio provided by its inputs.

 ## [ChorusNode ](soundnode/chorusnode.md)

Applies a chorus filter to the audio provided by its inputs.

 ## [FlangerNode ](soundnode/flangernode.md)

Applies a flanger filter to the audio provided by its inputs.

 ## [AddNoiseNode ](soundnode/addnoisenode.md)

Adds white noise to the audio provided by its inputs.

 ## [ModulationNode ](soundnode/modulationnode.md)

Applies either ring modulation or amplitude modulation to the audio provided by its inputs.

 # Recording Audio

 ## [RecordingNode ](soundnode/recordingnode.md)

Saves all audio produced by its inputs to a WAV file. 

 