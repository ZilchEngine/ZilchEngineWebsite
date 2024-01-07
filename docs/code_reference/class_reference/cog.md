 `Engine`

(NOTE) Game Object Composition class. This class is the foundational object for all dynamic objects in the game world. The Cog is a piece of logical interactive content and the primary mechanism game systems (Graphics, Physics, Etc.) provide functionality and communicate. A Cog can be anything from physical objects like trees, tanks, players to logical objects like teams, triggers, or AI objects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddComponentByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#addcomponentbyname-zero)|[ Actions](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#actions-zilch-engine-docu)|Object|[gamesession](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamesession.md)|
|[ AddComponentByType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#addcomponentbytype-zero)|[ Archetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#archetype-zilch-engine-do)| |[space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md)|
|[ AttachTo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#attachto-zilch-engine-doc)|[ BaseArchetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#basearchetype-zilch-engin)| | |
|[ AttachToPreserveLocal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#attachtopreservelocal-ze)|[ ChildCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#childcount-zilch-engine-d)| | |
|[ ClearArchetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#cleararchetype-void)|[ Children](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#children-zilch-engine-doc)| | |
|[ Clone](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#clone-zilch-engine-docume)|[ ComponentCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#componentcount-zilch-engi)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#cog-void)|[ EditorViewportHidden](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#editorviewporthidden-zer)| | |
|[ DebugDraw](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#debugdraw-void)|[ GameSession](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#gamesession-zilch-engine)| | |
|[ Destroy](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#destroy-void)|[ LevelSettings](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#levelsettings-zilch-engin)| | |
|[ Detach](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#detach-void)|[ Locked](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#locked-zilch-engine-docum)| | |
|[ DetachPreserveLocal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#detachpreservelocal-void)|[ MarkedForDestruction](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#markedfordestruction-zer)| | |
|[ DispatchDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#dispatchdown-void)|[ Name](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#name-zilch-engine-documen)| | |
|[ DispatchEvent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#dispatchevent-void)|[ ObjectViewHidden](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#objectviewhidden-zilch-en)| | |
|[ DispatchUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#dispatchup-void)|[ Parent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#parent-zilch-engine-docum)| | |
|[ FindAllChildrenByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#findallchildrenbyname-ze)|[ Persistent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#persistent-zilch-engine-d)| | |
|[ FindChildByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#findchildbyname-zilch-eng)|[ RuntimeId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#runtimeid-zilch-engine-do)| | |
|[ FindDirectChildByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#finddirectchildbyname-ze)|[ Space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#space-zilch-engine-docume)| | |
|[ FindNearestArchetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#findnearestarchetype-zer)|[ Transient](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#transient-zilch-engine-do)| | |
|[ FindNextInOrder](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#findnextinorder-zilch-eng)| | | |
|[ FindNextSibling](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#findnextsibling-zilch-eng)| | | |
|[ FindPreviousInOrder](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#findpreviousinorder-zero)| | | |
|[ FindPreviousSibling](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#findprevioussibling-zero)| | | |
|[ FindRoot](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#findroot-zilch-engine-doc)| | | |
|[ FindRootArchetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#findrootarchetype-zilch-e)| | | |
|[ GetComponentByIndex](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#getcomponentbyindex-zero)| | | |
|[ GetComponentByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#getcomponentbyname-zero)| | | |
|[ GetComponentIndex](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#getcomponentindex-zilch-e)| | | |
|[ IsAncestorOf](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#isancestorof-zilch-engine)| | | |
|[ IsDescendant](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#isdescendant-zilch-engine)| | | |
|[ IsDescendantOf](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#isdescendantof-zilch-engi)| | | |
|[ IsModifiedFromArchetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#ismodifiedfromarchetype)| | | |
|[ PlaceAfterSibling](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#placeaftersibling-void)| | | |
|[ PlaceBeforeSibling](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#placebeforesibling-void)| | | |
|[ RemoveComponentByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#removecomponentbyname-ze)| | | |
|[ RemoveComponentByType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#removecomponentbytype-ze)| | | |
|[ ReplaceChild](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#replacechild-void)| | | |
|[ SanitizeName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#sanitizename-zilch-engine)| | | |
|[ UploadToArchetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#uploadtoarchetype-void)| | | |


 #  Properties


---  
 #  Actions : [actions](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actions.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Actions : Actions


---  
 #  Archetype : [archetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/archetype.md)

> Getter / setter for Archetype.
> ``` lang=cpp, name=Nada
> var Archetype : Archetype


---  
 #  BaseArchetype : [archetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/archetype.md)

 `read-only`

> Returns the Archetype our Archetype inherits from.
> ``` lang=cpp, name=Nada
> var BaseArchetype : Archetype


---  
 #  ChildCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Returns the amount of children on this Cog. Note that this function has to iterate over all children to calculate the count.
> ``` lang=cpp, name=Nada
> var ChildCount : Integer


---  
 #  Children : [hierarchylistrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchylistrange.md)

 `read-only`

> Returns a range of all direct children on this Cog.
> ``` lang=cpp, name=Nada
> var Children : HierarchyListRange


---  
 #  ComponentCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Returns how many Components are on this Cog.
> ``` lang=cpp, name=Nada
> var ComponentCount : Integer


---  
 #  EditorViewportHidden : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Hidden from view used for editor.
> ``` lang=cpp, name=Nada
> var EditorViewportHidden : Boolean


---  
 #  GameSession : [gamesession](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamesession.md)

 `read-only`

> Get the GameSession that owns us and our Space.
> ``` lang=cpp, name=Nada
> var GameSession : GameSession


---  
 #  LevelSettings : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> Get the object named 'LevelSettings', a special convenience object where we can put general functionality for our Level.
> ``` lang=cpp, name=Nada
> var LevelSettings : Cog


---  
 #  Locked : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Not able to be modified or selected in the viewport.
> ``` lang=cpp, name=Nada
> var Locked : Boolean


---  
 #  MarkedForDestruction : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Has this Cog already been destroyed and is waiting for the frame to end (delayed destruction). This allows us to do custom logic when an object is still not null, but about to be destroyed (e.g. we don't want to render Cogs marked for deletion).
> ``` lang=cpp, name=Nada
> var MarkedForDestruction : Boolean


---  
 #  Name : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Name of the Object.
> ``` lang=cpp, name=Nada
> var Name : String


---  
 #  ObjectViewHidden : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If the object needs to not show up in the object view.
> ``` lang=cpp, name=Nada
> var ObjectViewHidden : Boolean


---  
 #  Parent : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> Get the parent of this object in the Hierarchy.
> ``` lang=cpp, name=Nada
> var Parent : Cog


---  
 #  Persistent : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Object will not be destroyed on level load or change.
> ``` lang=cpp, name=Nada
> var Persistent : Boolean


---  
 #  RuntimeId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Gets a unique integer for this object (used primarily for debugging)
> ``` lang=cpp, name=Nada
> var RuntimeId : Integer


---  
 #  Space : [space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md)

 `read-only`

> Returns the Space that this object lives in.
> ``` lang=cpp, name=Nada
> var Space : Space


---  
 #  Transient : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Object will not be saved.
> ``` lang=cpp, name=Nada
> var Transient : Boolean


---  
 #  Methods


---  
 #  AddComponentByName : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Add a component by name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function AddComponentByName(name : String) : Boolean
> ``` 


---  
 #  AddComponentByType : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Add a component of the given type.
> |Name|Type|Description|
> |---|---|---|
> |componentType|[boundtype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boundtype.md)| |
> ``` lang=cpp, name=Nada
> function AddComponentByType(componentType : BoundType) : Boolean
> ``` 


---  
 #  AttachTo : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Attach to a parent object and compute the new transform so that the objects are relative.
> |Name|Type|Description|
> |---|---|---|
> |parent|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function AttachTo(parent : Cog) : Boolean
> ``` 


---  
 #  AttachToPreserveLocal : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Attach to a parent object.
> |Name|Type|Description|
> |---|---|---|
> |parent|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function AttachToPreserveLocal(parent : Cog) : Boolean
> ``` 


---  
 #  ClearArchetype : Void

> Removes our association with the current Archetype.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ClearArchetype()
> ``` 


---  
 #  Clone : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Clones this cog. The cloned object will be parented to this objects parent (if it exists).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clone() : Cog
> ``` 


---  
 #  Cog : Void

 `constructor`

> Constructor / destructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Cog()
> ``` 


---  
 #  DebugDraw : Void

> Calls DebugDraw on all components in this cog.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DebugDraw()
> ``` 


---  
 #  Destroy : Void

> Queues the cog up for delayed destruction (at the end of the frame). If the object is marked as Protected, this will do nothing.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Destroy()
> ``` 


---  
 #  Detach : Void

> Detach from a parent object and compute the new transform so that the objects are relative.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Detach()
> ``` 


---  
 #  DetachPreserveLocal : Void

> Detach from a parent object.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DetachPreserveLocal()
> ``` 


---  
 #  DispatchDown : Void

> Dispatches an event down the tree on all children recursively (pre-order traversal)
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchDown(eventId : String, event : Event)
> ``` 


---  
 #  DispatchEvent : Void

> Dispatches an event on this object.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchEvent(eventId : String, event : Event)
> ``` 


---  
 #  DispatchUp : Void

> Dispatches an event up the tree on each parent recursively (pre-order traversal)
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchUp(eventId : String, event : Event)
> ``` 


---  
 #  FindAllChildrenByName : [hierarchynamerange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchynamerange.md)

> Returns a range of all children with the given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindAllChildrenByName(name : String) : HierarchyNameRange
> ``` 


---  
 #  FindChildByName : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Depth first search of all children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindChildByName(name : String) : Cog
> ``` 


---  
 #  FindDirectChildByName : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Checks only direct children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindDirectChildByName(name : String) : Cog
> ``` 


---  
 #  FindNearestArchetype : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Same as FindNearestParentArchetype except that it includes this Cog.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function FindNearestArchetype() : Cog
> ``` 


---  
 #  FindNextInOrder : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Finds the next Cog in depth first post-order.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function FindNextInOrder() : Cog
> ``` 


---  
 #  FindNextSibling : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Returns the sibling Cog after this in the parents child list. Returns null if it's the last child. If the Cog doesn't have a parent, it will return the Cog after it in the Space.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function FindNextSibling() : Cog
> ``` 


---  
 #  FindPreviousInOrder : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Finds the previous Cog in reverse depth first post-order (the opposite of FindNextInOrder).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function FindPreviousInOrder() : Cog
> ``` 


---  
 #  FindPreviousSibling : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Returns the sibling Cog before this in the parents child list. Returns null if it's the first child. If the Cog doesn't have a parent, it will return the Cog before it in the Space.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function FindPreviousSibling() : Cog
> ``` 


---  
 #  FindRoot : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Searches up the hierarchy for the root Cog.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function FindRoot() : Cog
> ``` 


---  
 #  FindRootArchetype : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Finds the top most Archetype in the Hierarchy.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function FindRootArchetype() : Cog
> ``` 


---  
 #  GetComponentByIndex : [component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)

> Returns the Component at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetComponentByIndex(index : Integer) : Component
> ``` 


---  
 #  GetComponentByName : [component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)

> Finds the Components with the given type name.
> |Name|Type|Description|
> |---|---|---|
> |componentTypeName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function GetComponentByName(componentTypeName : String) : Component
> ``` 


---  
 #  GetComponentIndex : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Finds the index of the given Component type. Returns uint max if the Component didn't exist.
> |Name|Type|Description|
> |---|---|---|
> |componentType|[boundtype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boundtype.md)| |
> ``` lang=cpp, name=Nada
> function GetComponentIndex(componentType : BoundType) : Integer
> ``` 


---  
 #  IsAncestorOf : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Returns whether or not we are an ancestor of the given Cog.
> |Name|Type|Description|
> |---|---|---|
> |descendant|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function IsAncestorOf(descendant : Cog) : Boolean
> ``` 


---  
 #  IsDescendant : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Returns whether or not the given cog is a descendant of us.
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function IsDescendant(cog : Cog) : Boolean
> ``` 


---  
 #  IsDescendantOf : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Returns whether or not we are a descendant of the given Cog.
> |Name|Type|Description|
> |---|---|---|
> |ancestor|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function IsDescendantOf(ancestor : Cog) : Boolean
> ``` 


---  
 #  IsModifiedFromArchetype : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Returns whether or not we have any local modifications from our Archetype. This does not account for properties with LocalModificationOverride (such as Transform modifications).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IsModifiedFromArchetype() : Boolean
> ``` 


---  
 #  PlaceAfterSibling : Void

> Moves this Cog after the given sibling. Assumes they have the same parent.
> |Name|Type|Description|
> |---|---|---|
> |sibling|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function PlaceAfterSibling(sibling : Cog)
> ``` 


---  
 #  PlaceBeforeSibling : Void

> Moves this Cog before the given sibling. Assumes they have the same parent.
> |Name|Type|Description|
> |---|---|---|
> |sibling|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function PlaceBeforeSibling(sibling : Cog)
> ``` 


---  
 #  RemoveComponentByName : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Remove a component by name. Returns true if the component existed.
> |Name|Type|Description|
> |---|---|---|
> |typeName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function RemoveComponentByName(typeName : String) : Boolean
> ``` 


---  
 #  RemoveComponentByType : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Remove a component by type. Returns true if the component existed.
> |Name|Type|Description|
> |---|---|---|
> |componentType|[boundtype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boundtype.md)| |
> ``` lang=cpp, name=Nada
> function RemoveComponentByType(componentType : BoundType) : Boolean
> ``` 


---  
 #  ReplaceChild : Void

> Places the new child at the same place as the old child in the Hierarchy. This detaches but does not destroy the old child.
> |Name|Type|Description|
> |---|---|---|
> |oldChild|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |newChild|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function ReplaceChild(oldChild : Cog, newChild : Cog)
> ``` 


---  
 #  SanitizeName : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `static`

> Cleans an object name of invalid runes.
> |Name|Type|Description|
> |---|---|---|
> |newName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function SanitizeName(newName : String) : String
> ``` 


---  
 #  UploadToArchetype : Void

> Upload this objects data to the archetype and marks this object as not modified. This function does not rebuild all other Cogs with the same Archetype. See ArchetypeRebuilder for more information about how to rebuild Archetypes.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function UploadToArchetype()
> ``` 


---  
 

 