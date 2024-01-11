 `Component` `Engine`



(NOTE) A component is an atomic piece of functionality that is composed into a Cog to form game objects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](component.md#component-void)|[ GameSession](component.md#gamesession-zilch-engine)|Object|[actionspace](actionspace.md)|
|[ DebugDraw](component.md#debugdraw-void)|[ LevelSettings](component.md#levelsettings-zilch-engin)| |[animationgraph](animationgraph.md)|
| |[ Owner](component.md#owner-zilch-engine-docume)| |[archetyped](archetyped.md)|
| |[ Space](component.md#space-zilch-engine-docume)| |[area](area.md)|
| | | |[audiosettings](audiosettings.md)|
| | | |[bone](bone.md)|
| | | |[camera](camera.md)|
| | | |[cameraviewport](cameraviewport.md)|
| | | |[collider](collider.md)|
| | | |ComponentProxy|
| | | |[contentconfig](contentconfig.md)|
| | | |[creationtool](creationtool.md)|
| | | |[customcollisioneventtracker](customcollisioneventtracker.md)|
| | | |[debugsettings](debugsettings.md)|
| | | |[defaultgamesetup](defaultgamesetup.md)|
| | | |[developerconfig](developerconfig.md)|
| | | |[dynamicmotor](dynamicmotor.md)|
| | | |[editorcameracontroller](editorcameracontroller.md)|
| | | |[editorconfig](editorconfig.md)|
| | | |[editorflags](editorflags.md)|
| | | |[editorsettings](editorsettings.md)|
| | | |[frameratesettings](frameratesettings.md)|
| | | |[gizmo](gizmo.md)|
| | | |[gizmocreator](gizmocreator.md)|
| | | |[gizmodrag](gizmodrag.md)|
| | | |[gizmospace](gizmospace.md)|
| | | |GjkDebug|
| | | |[graphical](graphical.md)|
| | | |[graphicsspace](graphicsspace.md)|
| | | |[griddraw](griddraw.md)|
| | | |[heightmap](heightmap.md)|
| | | |HeightMapAabbChecker|
| | | |HeightMapDebugDrawer|
| | | |[heightmaptool](heightmaptool.md)|
| | | |[hierarchy](hierarchy.md)|
| | | |[hierarchyspline](hierarchyspline.md)|
| | | |[ignorespaceeffects](ignorespaceeffects.md)|
| | | |[joint](joint.md)|
| | | |[jointconfigoverride](jointconfigoverride.md)|
| | | |[jointdebugdrawconfig](jointdebugdrawconfig.md)|
| | | |[jointlimit](jointlimit.md)|
| | | |[jointmotor](jointmotor.md)|
| | | |[jointspring](jointspring.md)|
| | | |LauncherConfig|
| | | |LauncherLegacySettings|
| | | |[linkid](linkid.md)|
| | | |[mainconfig](mainconfig.md)|
| | | |[manipulatortool](manipulatortool.md)|
| | | |[massoverride](massoverride.md)|
| | | |MeshDebug|
| | | |[mousecapture](mousecapture.md)|
| | | |[named](named.md)|
| | | |[netobject](netobject.md)|
| | | |[objectconnectingtool](objectconnectingtool.md)|
| | | |[objectlink](objectlink.md)|
| | | |[objectlinkanchor](objectlinkanchor.md)|
| | | |[objecttransformgizmo](objecttransformgizmo.md)|
| | | |[objecttransformtool](objecttransformtool.md)|
| | | |[orientation](orientation.md)|
| | | |[orientationbasisgizmo](orientationbasisgizmo.md)|
| | | |[particleanimator](particleanimator.md)|
| | | |[particleemitter](particleemitter.md)|
| | | |[physicscar](physicscar.md)|
| | | |[physicscarwheel](physicscarwheel.md)|
| | | |[physicscarwheelbasisgizmo](physicscarwheelbasisgizmo.md)|
| | | |[physicseffect](physicseffect.md)|
| | | |[physicsspace](physicsspace.md)|
| | | |[projectdescription](projectdescription.md)|
| | | |[projectsettings](projectsettings.md)|
| | | |[randomcontext](randomcontext.md)|
| | | |[reactive](reactive.md)|
| | | |[reactivespace](reactivespace.md)|
| | | |[recentprojects](recentprojects.md)|
| | | |[region](region.md)|
| | | |[revolutebasisgizmo](revolutebasisgizmo.md)|
| | | |[rigidbody](rigidbody.md)|
| | | |[rotategizmo](rotategizmo.md)|
| | | |[rotationbasisgizmo](rotationbasisgizmo.md)|
| | | |[scalegizmo](scalegizmo.md)|
| | | |[selectionicon](selectionicon.md)|
| | | |[selecttool](selecttool.md)|
| | | |[sharedcontent](sharedcontent.md)|
| | | |[simpleanimation](simpleanimation.md)|
| | | |[simplegizmobase](simplegizmobase.md)|
| | | |[simplesocket](simplesocket.md)|
| | | |[simplesound](simplesound.md)|
| | | |[skeleton](skeleton.md)|
| | | |[soundemitter](soundemitter.md)|
| | | |[soundlistener](soundlistener.md)|
| | | |[soundspace](soundspace.md)|
| | | |[spaceobjects](spaceobjects.md)|
| | | |SpringSystem|
| | | |SpringTools|
| | | |[texteditorconfig](texteditorconfig.md)|
| | | |[tileeditor2d](tileeditor2d.md)|
| | | |[tilemap](tilemap.md)|
| | | |TimeOfImpactDebug|
| | | |[timespace](timespace.md)|
| | | |[transform](transform.md)|
| | | |[translategizmo](translategizmo.md)|
| | | |[uilayout](uilayout.md)|
| | | |[uiwidgetcomponenthierarchy](uiwidgetcomponenthierarchy.md)|
| | | |[userconfig](userconfig.md)|
| | | |[webrequester](webrequester.md)|
| | | |[windowlaunchsettings](windowlaunchsettings.md)|
| | | |[nadacomponent](nadacomponent.md)|
| | | |[nadapluginconfig](nadapluginconfig.md)|


 #  Properties


---  
 #  GameSession : [gamesession](gamesession.md)

 `read-only`

> Get the GameSession that owns us and our space.
> ```TS:Nada
> var GameSession : GameSession


---  
 #  LevelSettings : [cog](cog.md)

 `read-only`

> Get the object named 'LevelSettings', a special object where we can put components for our level.
> ```TS:Nada
> var LevelSettings : Cog


---  
 #  Owner : [cog](cog.md)

 `read-only`

> Get the Cog this Component is owned by (not the parent of this composition).
> ```TS:Nada
> var Owner : Cog


---  
 #  Space : [space](space.md)

 `read-only`

> The Space where the object is located.
> ```TS:Nada
> var Space : Space


---  
 #  Methods


---  
 #  Component : Void

 `constructor`

> Constructor / Destructor.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Component()
> ``` 


---  
 #  DebugDraw : Void

> Base debug draw for a component. Special for the each type of component.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function DebugDraw()
> ``` 


---  
 

 