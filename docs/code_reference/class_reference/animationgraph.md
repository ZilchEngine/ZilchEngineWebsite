 `Component` `Engine`



(NOTE) The AnimationGraph component controls animation for an individual game object. It stores all needed per instance (vs what is shared in the animation resource) manages the current time and enumerates the animation sets. The AnimationGraph can animate multiple child objects and properties enabling bone animation, and other hierarchical animations.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](animationgraph.md#animationgraph-void)|[ Active](animationgraph.md#active-zilch-engine-docum)|[component](component.md)| |
|[ CreateBasicNode](animationgraph.md#createbasicnode-zilch-eng)|[ ActiveNode](animationgraph.md#activenode-zilch-engine-d)| | |
|[ CreateChainNode](animationgraph.md#createchainnode-zilch-eng)|[ TimeScale](animationgraph.md#timescale-zilch-engine-do)| | |
|[ CreateCrossBlendNode](animationgraph.md#createcrossblendnode-zer)| | | |
|[ CreateDirectBlendNode](animationgraph.md#createdirectblendnode-ze)| | | |
|[ CreateSelectiveNode](animationgraph.md#createselectivenode-zero)| | | |
|[ IsPlayingInGraph](animationgraph.md#isplayingingraph-zilch-en)| | | |
|[ PrintGraph](animationgraph.md#printgraph-void)| | | |
|[ Update](animationgraph.md#update-void)| | | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> Is the animGraph animating?
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  ActiveNode : [animationnode](animationnode.md)

> The current root animation node.
> ``` lang=cpp, name=Nada
> var ActiveNode : AnimationNode


---  
 #  TimeScale : [real](../nada_base_types/real.md)

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
 #  CreateBasicNode : [basicanimation](basicanimation.md)

> Node creation functions.
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](animation.md)| |
> |mode|[AnimationPlayMode](../enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Nada
> function CreateBasicNode(animation : Animation, mode : AnimationPlayMode) : BasicAnimation
> ``` 


---  
 #  CreateChainNode : [chainnode](chainnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateChainNode() : ChainNode
> ``` 


---  
 #  CreateCrossBlendNode : [crossblend](crossblend.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateCrossBlendNode() : CrossBlend
> ``` 


---  
 #  CreateDirectBlendNode : [directblend](directblend.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateDirectBlendNode() : DirectBlend
> ``` 


---  
 #  CreateSelectiveNode : [selectivenode](selectivenode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateSelectiveNode() : SelectiveNode
> ``` 


---  
 #  IsPlayingInGraph : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](animation.md)| |
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
> |dt|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Update(dt : Real)
> ``` 


---  
 

 