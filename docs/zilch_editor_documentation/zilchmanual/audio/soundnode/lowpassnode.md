The [ LowPassNode ](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/lowpassnode.md) collects audio data from all of its inputs and applies a low pass filter to it before passing it along to its outputs.

 # Common Uses

- Making audio sound muffled
- Combining with white noise and other audio filters to create wind or other sound effects

 # Using the LowPassNode 

Low pass filters leave low frequencies untouched while silencing high frequencies above their cutoff frequency. The only property on the LowPassNode is the `CutoffFrequency`, which sets the frequency at which the filter starts to take effect.

---
 # Related Materials
 ## Manual
- [soudnode_overview](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundnode/soudnode_overview.md)
- [bandpassnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundnode/bandpassnode.md)
- [highpassnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundnode/highpassnode.md)

 ## Code Reference
- [ LowPassNode ](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/lowpassnode.md) 

 