 `Component` `Engine`



(NOTE) The AnimationGraph component controls animation for an individual game object. It stores all needed per instance (vs what is shared in the animation resource) manages the current time and enumerates the animation sets. The AnimationGraph can animate multiple child objects and properties enabling bone animation, and other hierarchical animations.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#animationgraph-void)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#active-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ CreateBasicNode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#createbasicnode-zilch-eng)|[ ActiveNode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#activenode-zilch-engine-d)| | |
|[ CreateChainNode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#createchainnode-zilch-eng)|[ TimeScale](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#timescale-zilch-engine-do)| | |
|[ CreateCrossBlendNode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#createcrossblendnode-zer)| | | |
|[ CreateDirectBlendNode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#createdirectblendnode-ze)| | | |
|[ CreateSelectiveNode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#createselectivenode-zero)| | | |
|[ IsPlayingInGraph](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#isplayingingraph-zilch-en)| | | |
|[ PrintGraph](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#printgraph-void)| | | |
|[ Update](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationgraph.md#update-void)| | | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is the animGraph animating?
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  ActiveNode : [animationnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md)

> The current root animation node.
> ``` lang=cpp, name=Nada
> var ActiveNode : AnimationNode


---  
 #  TimeScale : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> A scalar to the entire animation graph.
> ``` lang=cpp, name=Nada
> var TimeScale : Real


---  
 #  Methods


---  
 #  AnimationGraph : Void

 `constructor`

> Constructor / destructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function AnimationGraph()
> ``` 


---  
 #  CreateBasicNode : [basicanimation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basicanimation.md)

> Node creation functions.
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animation.md)| |
> |mode|[AnimationPlayMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Nada
> function CreateBasicNode(animation : Animation, mode : AnimationPlayMode) : BasicAnimation
> ``` 


---  
 #  CreateChainNode : [chainnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/chainnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateChainNode() : ChainNode
> ``` 


---  
 #  CreateCrossBlendNode : [crossblend](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/crossblend.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateCrossBlendNode() : CrossBlend
> ``` 


---  
 #  CreateDirectBlendNode : [directblend](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/directblend.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateDirectBlendNode() : DirectBlend
> ``` 


---  
 #  CreateSelectiveNode : [selectivenode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/selectivenode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateSelectiveNode() : SelectiveNode
> ``` 


---  
 #  IsPlayingInGraph : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animation.md)| |
> ``` lang=cpp, name=Nada
> function IsPlayingInGraph(animation : Animation) : Boolean
> ``` 


---  
 #  PrintGraph : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PrintGraph()
> ``` 


---  
 #  Update : Void

> Updates the root node on each from and applies it to the object tree.
> |Name|Type|Description|
> |---|---|---|
> |dt|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Update(dt : Real)
> ``` 


---  
 

 