 `Engine`

(NOTE) Game Object Composition class. This class is the foundational object for all dynamic objects in the game world. The Cog is a piece of logical interactive content and the primary mechanism game systems (Graphics, Physics, Etc.) provide functionality and communicate. A Cog can be anything from physical objects like trees, tanks, players to logical objects like teams, triggers, or AI objects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddComponentByName](cog.md#addcomponentbyname-zero)|[ Actions](cog.md#actions-zilch-engine-docu)|Object|[gamesession](gamesession.md)|
|[ AddComponentByType](cog.md#addcomponentbytype-zero)|[ Archetype](cog.md#archetype-zilch-engine-do)| |[space](space.md)|
|[ AttachTo](cog.md#attachto-zilch-engine-doc)|[ BaseArchetype](cog.md#basearchetype-zilch-engin)| | |
|[ AttachToPreserveLocal](cog.md#attachtopreservelocal-ze)|[ ChildCount](cog.md#childcount-zilch-engine-d)| | |
|[ ClearArchetype](cog.md#cleararchetype-void)|[ Children](cog.md#children-zilch-engine-doc)| | |
|[ Clone](cog.md#clone-zilch-engine-docume)|[ ComponentCount](cog.md#componentcount-zilch-engi)| | |
|[ Constructor](cog.md#cog-void)|[ EditorViewportHidden](cog.md#editorviewporthidden-zer)| | |
|[ DebugDraw](cog.md#debugdraw-void)|[ GameSession](cog.md#gamesession-zilch-engine)| | |
|[ Destroy](cog.md#destroy-void)|[ LevelSettings](cog.md#levelsettings-zilch-engin)| | |
|[ Detach](cog.md#detach-void)|[ Locked](cog.md#locked-zilch-engine-docum)| | |
|[ DetachPreserveLocal](cog.md#detachpreservelocal-void)|[ MarkedForDestruction](cog.md#markedfordestruction-zer)| | |
|[ DispatchDown](cog.md#dispatchdown-void)|[ Name](cog.md#name-zilch-engine-documen)| | |
|[ DispatchEvent](cog.md#dispatchevent-void)|[ ObjectViewHidden](cog.md#objectviewhidden-zilch-en)| | |
|[ DispatchUp](cog.md#dispatchup-void)|[ Parent](cog.md#parent-zilch-engine-docum)| | |
|[ FindAllChildrenByName](cog.md#findallchildrenbyname-ze)|[ Persistent](cog.md#persistent-zilch-engine-d)| | |
|[ FindChildByName](cog.md#findchildbyname-zilch-eng)|[ RuntimeId](cog.md#runtimeid-zilch-engine-do)| | |
|[ FindDirectChildByName](cog.md#finddirectchildbyname-ze)|[ Space](cog.md#space-zilch-engine-docume)| | |
|[ FindNearestArchetype](cog.md#findnearestarchetype-zer)|[ Transient](cog.md#transient-zilch-engine-do)| | |
|[ FindNextInOrder](cog.md#findnextinorder-zilch-eng)| | | |
|[ FindNextSibling](cog.md#findnextsibling-zilch-eng)| | | |
|[ FindPreviousInOrder](cog.md#findpreviousinorder-zero)| | | |
|[ FindPreviousSibling](cog.md#findprevioussibling-zero)| | | |
|[ FindRoot](cog.md#findroot-zilch-engine-doc)| | | |
|[ FindRootArchetype](cog.md#findrootarchetype-zilch-e)| | | |
|[ GetComponentByIndex](cog.md#getcomponentbyindex-zero)| | | |
|[ GetComponentByName](cog.md#getcomponentbyname-zero)| | | |
|[ GetComponentIndex](cog.md#getcomponentindex-zilch-e)| | | |
|[ IsAncestorOf](cog.md#isancestorof-zilch-engine)| | | |
|[ IsDescendant](cog.md#isdescendant-zilch-engine)| | | |
|[ IsDescendantOf](cog.md#isdescendantof-zilch-engi)| | | |
|[ IsModifiedFromArchetype](cog.md#ismodifiedfromarchetype)| | | |
|[ PlaceAfterSibling](cog.md#placeaftersibling-void)| | | |
|[ PlaceBeforeSibling](cog.md#placebeforesibling-void)| | | |
|[ RemoveComponentByName](cog.md#removecomponentbyname-ze)| | | |
|[ RemoveComponentByType](cog.md#removecomponentbytype-ze)| | | |
|[ ReplaceChild](cog.md#replacechild-void)| | | |
|[ SanitizeName](cog.md#sanitizename-zilch-engine)| | | |
|[ UploadToArchetype](cog.md#uploadtoarchetype-void)| | | |


 #  Properties


---  
 #  Actions : [actions](actions.md)

 `read-only`

> 
> ```TS:Nada
> var Actions : Actions


---  
 #  Archetype : [archetype](archetype.md)

> Getter / setter for Archetype.
> ```TS:Nada
> var Archetype : Archetype


---  
 #  BaseArchetype : [archetype](archetype.md)

 `read-only`

> Returns the Archetype our Archetype inherits from.
> ```TS:Nada
> var BaseArchetype : Archetype


---  
 #  ChildCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the amount of children on this Cog. Note that this function has to iterate over all children to calculate the count.
> ```TS:Nada
> var ChildCount : Integer


---  
 #  Children : [hierarchylistrange](hierarchylistrange.md)

 `read-only`

> Returns a range of all direct children on this Cog.
> ```TS:Nada
> var Children : HierarchyListRange


---  
 #  ComponentCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns how many Components are on this Cog.
> ```TS:Nada
> var ComponentCount : Integer


---  
 #  EditorViewportHidden : [boolean](../nada_base_types/boolean.md)

> Hidden from view used for editor.
> ```TS:Nada
> var EditorViewportHidden : Boolean


---  
 #  GameSession : [gamesession](gamesession.md)

 `read-only`

> Get the GameSession that owns us and our Space.
> ```TS:Nada
> var GameSession : GameSession


---  
 #  LevelSettings : [cog](cog.md)

 `read-only`

> Get the object named 'LevelSettings', a special convenience object where we can put general functionality for our Level.
> ```TS:Nada
> var LevelSettings : Cog


---  
 #  Locked : [boolean](../nada_base_types/boolean.md)

> Not able to be modified or selected in the viewport.
> ```TS:Nada
> var Locked : Boolean


---  
 #  MarkedForDestruction : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Has this Cog already been destroyed and is waiting for the frame to end (delayed destruction). This allows us to do custom logic when an object is still not null, but about to be destroyed (e.g. we don't want to render Cogs marked for deletion).
> ```TS:Nada
> var MarkedForDestruction : Boolean


---  
 #  Name : [string](../nada_base_types/string.md)

> Name of the Object.
> ```TS:Nada
> var Name : String


---  
 #  ObjectViewHidden : [boolean](../nada_base_types/boolean.md)

> If the object needs to not show up in the object view.
> ```TS:Nada
> var ObjectViewHidden : Boolean


---  
 #  Parent : [cog](cog.md)

 `read-only`

> Get the parent of this object in the Hierarchy.
> ```TS:Nada
> var Parent : Cog


---  
 #  Persistent : [boolean](../nada_base_types/boolean.md)

> Object will not be destroyed on level load or change.
> ```TS:Nada
> var Persistent : Boolean


---  
 #  RuntimeId : [integer](../nada_base_types/integer.md)

 `read-only`

> Gets a unique integer for this object (used primarily for debugging)
> ```TS:Nada
> var RuntimeId : Integer


---  
 #  Space : [space](space.md)

 `read-only`

> Returns the Space that this object lives in.
> ```TS:Nada
> var Space : Space


---  
 #  Transient : [boolean](../nada_base_types/boolean.md)

> Object will not be saved.
> ```TS:Nada
> var Transient : Boolean


---  
 #  Methods


---  
 #  AddComponentByName : [boolean](../nada_base_types/boolean.md)

> Add a component by name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function AddComponentByName(name : String) : Boolean
> ``` 


---  
 #  AddComponentByType : [boolean](../nada_base_types/boolean.md)

> Add a component of the given type.
> |Name|Type|Description|
> |---|---|---|
> |componentType|[boundtype](../nada_base_types/boundtype.md)| |
> ```TS:Nada
> function AddComponentByType(componentType : BoundType) : Boolean
> ``` 


---  
 #  AttachTo : [boolean](../nada_base_types/boolean.md)

> Attach to a parent object and compute the new transform so that the objects are relative.
> |Name|Type|Description|
> |---|---|---|
> |parent|[cog](cog.md)| |
> ```TS:Nada
> function AttachTo(parent : Cog) : Boolean
> ``` 


---  
 #  AttachToPreserveLocal : [boolean](../nada_base_types/boolean.md)

> Attach to a parent object.
> |Name|Type|Description|
> |---|---|---|
> |parent|[cog](cog.md)| |
> ```TS:Nada
> function AttachToPreserveLocal(parent : Cog) : Boolean
> ``` 


---  
 #  ClearArchetype : Void

> Removes our association with the current Archetype.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ClearArchetype()
> ``` 


---  
 #  Clone : [cog](cog.md)

> Clones this cog. The cloned object will be parented to this objects parent (if it exists).
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Clone() : Cog
> ``` 


---  
 #  Cog : Void

 `constructor`

> Constructor / destructor.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Cog()
> ``` 


---  
 #  DebugDraw : Void

> Calls DebugDraw on all components in this cog.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function DebugDraw()
> ``` 


---  
 #  Destroy : Void

> Queues the cog up for delayed destruction (at the end of the frame). If the object is marked as Protected, this will do nothing.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Destroy()
> ``` 


---  
 #  Detach : Void

> Detach from a parent object and compute the new transform so that the objects are relative.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Detach()
> ``` 


---  
 #  DetachPreserveLocal : Void

> Detach from a parent object.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function DetachPreserveLocal()
> ``` 


---  
 #  DispatchDown : Void

> Dispatches an event down the tree on all children recursively (pre-order traversal)
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[event](event.md)| |
> ```TS:Nada
> function DispatchDown(eventId : String, event : Event)
> ``` 


---  
 #  DispatchEvent : Void

> Dispatches an event on this object.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[event](event.md)| |
> ```TS:Nada
> function DispatchEvent(eventId : String, event : Event)
> ``` 


---  
 #  DispatchUp : Void

> Dispatches an event up the tree on each parent recursively (pre-order traversal)
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[event](event.md)| |
> ```TS:Nada
> function DispatchUp(eventId : String, event : Event)
> ``` 


---  
 #  FindAllChildrenByName : [hierarchynamerange](hierarchynamerange.md)

> Returns a range of all children with the given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function FindAllChildrenByName(name : String) : HierarchyNameRange
> ``` 


---  
 #  FindChildByName : [cog](cog.md)

> Depth first search of all children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function FindChildByName(name : String) : Cog
> ``` 


---  
 #  FindDirectChildByName : [cog](cog.md)

> Checks only direct children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function FindDirectChildByName(name : String) : Cog
> ``` 


---  
 #  FindNearestArchetype : [cog](cog.md)

> Same as FindNearestParentArchetype except that it includes this Cog.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function FindNearestArchetype() : Cog
> ``` 


---  
 #  FindNextInOrder : [cog](cog.md)

> Finds the next Cog in depth first post-order.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function FindNextInOrder() : Cog
> ``` 


---  
 #  FindNextSibling : [cog](cog.md)

> Returns the sibling Cog after this in the parents child list. Returns null if it's the last child. If the Cog doesn't have a parent, it will return the Cog after it in the Space.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function FindNextSibling() : Cog
> ``` 


---  
 #  FindPreviousInOrder : [cog](cog.md)

> Finds the previous Cog in reverse depth first post-order (the opposite of FindNextInOrder).
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function FindPreviousInOrder() : Cog
> ``` 


---  
 #  FindPreviousSibling : [cog](cog.md)

> Returns the sibling Cog before this in the parents child list. Returns null if it's the first child. If the Cog doesn't have a parent, it will return the Cog before it in the Space.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function FindPreviousSibling() : Cog
> ``` 


---  
 #  FindRoot : [cog](cog.md)

> Searches up the hierarchy for the root Cog.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function FindRoot() : Cog
> ``` 


---  
 #  FindRootArchetype : [cog](cog.md)

> Finds the top most Archetype in the Hierarchy.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function FindRootArchetype() : Cog
> ``` 


---  
 #  GetComponentByIndex : [component](component.md)

> Returns the Component at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetComponentByIndex(index : Integer) : Component
> ``` 


---  
 #  GetComponentByName : [component](component.md)

> Finds the Components with the given type name.
> |Name|Type|Description|
> |---|---|---|
> |componentTypeName|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function GetComponentByName(componentTypeName : String) : Component
> ``` 


---  
 #  GetComponentIndex : [integer](../nada_base_types/integer.md)

> Finds the index of the given Component type. Returns uint max if the Component didn't exist.
> |Name|Type|Description|
> |---|---|---|
> |componentType|[boundtype](../nada_base_types/boundtype.md)| |
> ```TS:Nada
> function GetComponentIndex(componentType : BoundType) : Integer
> ``` 


---  
 #  IsAncestorOf : [boolean](../nada_base_types/boolean.md)

> Returns whether or not we are an ancestor of the given Cog.
> |Name|Type|Description|
> |---|---|---|
> |descendant|[cog](cog.md)| |
> ```TS:Nada
> function IsAncestorOf(descendant : Cog) : Boolean
> ``` 


---  
 #  IsDescendant : [boolean](../nada_base_types/boolean.md)

> Returns whether or not the given cog is a descendant of us.
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](cog.md)| |
> ```TS:Nada
> function IsDescendant(cog : Cog) : Boolean
> ``` 


---  
 #  IsDescendantOf : [boolean](../nada_base_types/boolean.md)

> Returns whether or not we are a descendant of the given Cog.
> |Name|Type|Description|
> |---|---|---|
> |ancestor|[cog](cog.md)| |
> ```TS:Nada
> function IsDescendantOf(ancestor : Cog) : Boolean
> ``` 


---  
 #  IsModifiedFromArchetype : [boolean](../nada_base_types/boolean.md)

> Returns whether or not we have any local modifications from our Archetype. This does not account for properties with LocalModificationOverride (such as Transform modifications).
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function IsModifiedFromArchetype() : Boolean
> ``` 


---  
 #  PlaceAfterSibling : Void

> Moves this Cog after the given sibling. Assumes they have the same parent.
> |Name|Type|Description|
> |---|---|---|
> |sibling|[cog](cog.md)| |
> ```TS:Nada
> function PlaceAfterSibling(sibling : Cog)
> ``` 


---  
 #  PlaceBeforeSibling : Void

> Moves this Cog before the given sibling. Assumes they have the same parent.
> |Name|Type|Description|
> |---|---|---|
> |sibling|[cog](cog.md)| |
> ```TS:Nada
> function PlaceBeforeSibling(sibling : Cog)
> ``` 


---  
 #  RemoveComponentByName : [boolean](../nada_base_types/boolean.md)

> Remove a component by name. Returns true if the component existed.
> |Name|Type|Description|
> |---|---|---|
> |typeName|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function RemoveComponentByName(typeName : String) : Boolean
> ``` 


---  
 #  RemoveComponentByType : [boolean](../nada_base_types/boolean.md)

> Remove a component by type. Returns true if the component existed.
> |Name|Type|Description|
> |---|---|---|
> |componentType|[boundtype](../nada_base_types/boundtype.md)| |
> ```TS:Nada
> function RemoveComponentByType(componentType : BoundType) : Boolean
> ``` 


---  
 #  ReplaceChild : Void

> Places the new child at the same place as the old child in the Hierarchy. This detaches but does not destroy the old child.
> |Name|Type|Description|
> |---|---|---|
> |oldChild|[cog](cog.md)| |
> |newChild|[cog](cog.md)| |
> ```TS:Nada
> function ReplaceChild(oldChild : Cog, newChild : Cog)
> ``` 


---  
 #  SanitizeName : [string](../nada_base_types/string.md)

 `static`

> Cleans an object name of invalid runes.
> |Name|Type|Description|
> |---|---|---|
> |newName|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function SanitizeName(newName : String) : String
> ``` 


---  
 #  UploadToArchetype : Void

> Upload this objects data to the archetype and marks this object as not modified. This function does not rebuild all other Cogs with the same Archetype. See ArchetypeRebuilder for more information about how to rebuild Archetypes.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function UploadToArchetype()
> ``` 


---  
 

 