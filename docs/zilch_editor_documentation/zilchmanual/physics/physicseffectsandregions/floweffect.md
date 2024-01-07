The [FlowEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md) component applies forces to make an object move at a target speed in a given direction. This is often used to make an object move in the flow of another, such as a river or a tractor beam.



![FlowEffect](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46701.png)


Unlike a [ForceEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions/forceeffect.md) which applies a constant force in a direction, FlowEffect applies a variable force to make an object move at a constant speed in the flow direction. MaxFlowForce  allows the user to control how much force can be applied to reach this target speed. This can also be thought of as controlling the acceleration of objects within the field. Note: the flow portion of the effect only affects movement in the flow direction, not in the inward force direction.

Additionally, FlowEffect has the AttractToFlowCenter checkBox property to pull objects towards the flow center. This attractional force is similarly defined by a target speed and a max force. Note: this force only affects movement in the inward direction, not in the flow direction.

 #  Application Modes
FlowEffect is only expected to be used as a [Region](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/region.md) effect. Other application modes are undefined.

---
 #  Related Materials
 ##  Manual
- [physicseffectsandregions.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions.md)
- [forceeffect.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions/forceeffect.md)

 ##  Reference
- [FlowEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md)
- [ForceEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/forceeffect.md)
- [PhysicsEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md)
- [Region](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/region.md)
 

 