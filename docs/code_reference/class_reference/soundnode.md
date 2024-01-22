 `Sound`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[AddInputNode](soundnode.md#addinputnode-void)|[AutoCollapse](soundnode.md#autocollapse-zilch-engine)|[referencecountedeventobject](referencecountedeventobject.md)|[additivesynthnode](additivesynthnode.md)|
|[InsertNodeAfter](soundnode.md#insertnodeafter-void)|[BypassPercent](soundnode.md#bypasspercent-zilch-engin)| |[addnoisenode](addnoisenode.md)|
|[InsertNodeBefore](soundnode.md#insertnodebefore-void)|[BypassValue](soundnode.md#bypassvalue-zilch-engine)| |[bandpassnode](bandpassnode.md)|
|[RemoveAllInputs](soundnode.md#removeallinputs-void)|[HasInputs](soundnode.md#hasinputs-zilch-engine-do)| |[chorusnode](chorusnode.md)|
|[RemoveAllOutputs](soundnode.md#removealloutputs-void)|[HasOutputs](soundnode.md#hasoutputs-zilch-engine-d)| |[compressornode](compressornode.md)|
|[RemoveAndAttachInputsToOutputs](soundnode.md#removeandattachinputstoo)|[InputCount](soundnode.md#inputcount-zilch-engine-d)| |[customaudionode](customaudionode.md)|
|[RemoveInputNode](soundnode.md#removeinputnode-void)|[OutputCount](soundnode.md#outputcount-zilch-engine)| |[delaynode](delaynode.md)|
|[ReplaceWith](soundnode.md#replacewith-void)| | |[equalizernode](equalizernode.md)|
| | | |[expandernode](expandernode.md)|
| | | |[flangernode](flangernode.md)|
| | | |[generatedwavenode](generatedwavenode.md)|
| | | |[granularsynthnode](granularsynthnode.md)|
| | | |[highpassnode](highpassnode.md)|
| | | |[lowpassnode](lowpassnode.md)|
| | | |[microphoneinputnode](microphoneinputnode.md)|
| | | |[modulationnode](modulationnode.md)|
| | | |[panningnode](panningnode.md)|
| | | |[pitchnode](pitchnode.md)|
| | | |[recordingnode](recordingnode.md)|
| | | |[reverbnode](reverbnode.md)|
| | | |[saveaudionode](saveaudionode.md)|
| | | |[volumenode](volumenode.md)|


 #  Properties


---  
 #  AutoCollapse : [boolean](../nada_base_types/boolean.md)

> If true, this node will automatically remove itself from the graph when its last input node is removed.
> ```TS:Nada
> var AutoCollapse : Boolean


---  
 #  BypassPercent : [real](../nada_base_types/real.md)

> DEPRECATED The BypassValue property should be used instead.
> ```TS:Nada
> var BypassPercent : Real


---  
 #  BypassValue : [real](../nada_base_types/real.md)

> The percentage of output (0 to 1.0) that should skip whatever processing the node does.
> ```TS:Nada
> var BypassValue : Real


---  
 #  HasInputs : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Will be true if this node has any input nodes.
> ```TS:Nada
> var HasInputs : Boolean


---  
 #  HasOutputs : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Will be true if this node has any output nodes.
> ```TS:Nada
> var HasOutputs : Boolean


---  
 #  InputCount : [integer](../nada_base_types/integer.md)

 `read-only`

> The number of input nodes that are currently attached to this node.
> ```TS:Nada
> var InputCount : Integer


---  
 #  OutputCount : [integer](../nada_base_types/integer.md)

 `read-only`

> The number of output nodes that are currently attached to this node.
> ```TS:Nada
> var OutputCount : Integer


---  
 #  Methods


---  
 #  AddInputNode : Void

> Adds the passed in node to this node's inputs.
> |Name|Type|Description|
> |---|---|---|
> |node|[soundnode](soundnode.md)| |
> ```TS:Nada
> function AddInputNode(node : SoundNode)
> ``` 


---  
 #  InsertNodeAfter : Void

> Inserts the passed in node after this node in the signal path, placing it between this node and any nodes which were connected to this node's output.
> |Name|Type|Description|
> |---|---|---|
> |node|[soundnode](soundnode.md)| |
> ```TS:Nada
> function InsertNodeAfter(node : SoundNode)
> ``` 


---  
 #  InsertNodeBefore : Void

> Inserts the passed in node before this node in the signal path, placing it between this node and any nodes which were connected to this node as inputs.
> |Name|Type|Description|
> |---|---|---|
> |node|[soundnode](soundnode.md)| |
> ```TS:Nada
> function InsertNodeBefore(node : SoundNode)
> ``` 


---  
 #  RemoveAllInputs : Void

> Removes the connections between this node and all of its input nodes.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RemoveAllInputs()
> ``` 


---  
 #  RemoveAllOutputs : Void

> Removes the connections between this node and all of its output nodes, disconnecting this node from the graph. If this node has no inputs it will be deleted when no longer referenced.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RemoveAllOutputs()
> ``` 


---  
 #  RemoveAndAttachInputsToOutputs : Void

> Removes this node from the graph by disconnecting it from all inputs and outputs and attaching the input nodes to the output nodes, keeping the rest of the graph intact. This node will be deleted when it is no longer referenced.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RemoveAndAttachInputsToOutputs()
> ``` 


---  
 #  RemoveInputNode : Void

> Removes the node passed in as a parameter from this node's inputs.
> |Name|Type|Description|
> |---|---|---|
> |node|[soundnode](soundnode.md)| |
> ```TS:Nada
> function RemoveInputNode(node : SoundNode)
> ``` 


---  
 #  ReplaceWith : Void

> Replaces this node in the graph with the node passed in as a parameter. This node will be deleted when it is no longer referenced.
> |Name|Type|Description|
> |---|---|---|
> |node|[soundnode](soundnode.md)| |
> ```TS:Nada
> function ReplaceWith(node : SoundNode)
> ``` 


---  
 

 