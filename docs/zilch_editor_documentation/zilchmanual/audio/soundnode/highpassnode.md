The [ HighPassNode ](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/highpassnode.md) collects audio data from all of its inputs and applies a high pass filter to it before passing it along to its outputs. 

 # Common Uses

- Removing excessive low frequencies
- Combining with white noise and other audio filters to create wind or other sound effects

 # Using the HighPassNode

High pass filters leave high frequencies untouched while silencing low frequencies below their cutoff frequency. The only property on the HighPassNode is the `CutoffFrequency`, which sets the frequency at which the filter starts to take effect.

___
 # Related Materials
 ## Manual
- [soudnode_overview](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundnode/soudnode_overview.md)
- [bandpassnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundnode/bandpassnode.md)
- [lowpassnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundnode/lowpassnode.md)

 ## Code Reference
- [ HighPassNode ](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/highpassnode.md) 

 