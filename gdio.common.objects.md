<a name='assembly'></a>
# gdio.common.objects

## Contents

- [COLLISION_EVENT](#T-gdio-common-objects-COLLISION_EVENT 'gdio.common.objects.COLLISION_EVENT')
  - [COLLISION_ENTER](#F-gdio-common-objects-COLLISION_EVENT-COLLISION_ENTER 'gdio.common.objects.COLLISION_EVENT.COLLISION_ENTER')
  - [COLLISION_EXIT](#F-gdio-common-objects-COLLISION_EVENT-COLLISION_EXIT 'gdio.common.objects.COLLISION_EVENT.COLLISION_EXIT')
  - [COLLISION_STAY](#F-gdio-common-objects-COLLISION_EVENT-COLLISION_STAY 'gdio.common.objects.COLLISION_EVENT.COLLISION_STAY')
- [Collider](#T-gdio-common-objects-Collider 'gdio.common.objects.Collider')
  - [attachedRigidbody](#F-gdio-common-objects-Collider-attachedRigidbody 'gdio.common.objects.Collider.attachedRigidbody')
  - [bounds](#F-gdio-common-objects-Collider-bounds 'gdio.common.objects.Collider.bounds')
  - [contactOffset](#F-gdio-common-objects-Collider-contactOffset 'gdio.common.objects.Collider.contactOffset')
  - [enabled](#F-gdio-common-objects-Collider-enabled 'gdio.common.objects.Collider.enabled')
  - [isTrigger](#F-gdio-common-objects-Collider-isTrigger 'gdio.common.objects.Collider.isTrigger')
  - [material](#F-gdio-common-objects-Collider-material 'gdio.common.objects.Collider.material')
  - [sharedMaterial](#F-gdio-common-objects-Collider-sharedMaterial 'gdio.common.objects.Collider.sharedMaterial')
- [Collision](#T-gdio-common-objects-Collision 'gdio.common.objects.Collision')
  - [CollisionType](#F-gdio-common-objects-Collision-CollisionType 'gdio.common.objects.Collision.CollisionType')
  - [HierarchyPath](#F-gdio-common-objects-Collision-HierarchyPath 'gdio.common.objects.Collision.HierarchyPath')
  - [Timestamp](#F-gdio-common-objects-Collision-Timestamp 'gdio.common.objects.Collision.Timestamp')
  - [contactCount](#F-gdio-common-objects-Collision-contactCount 'gdio.common.objects.Collision.contactCount')
  - [contacts](#F-gdio-common-objects-Collision-contacts 'gdio.common.objects.Collision.contacts')
  - [gameObject](#F-gdio-common-objects-Collision-gameObject 'gdio.common.objects.Collision.gameObject')
  - [impulse](#F-gdio-common-objects-Collision-impulse 'gdio.common.objects.Collision.impulse')
  - [relativeVelocity](#F-gdio-common-objects-Collision-relativeVelocity 'gdio.common.objects.Collision.relativeVelocity')
  - [rigidbody](#F-gdio-common-objects-Collision-rigidbody 'gdio.common.objects.Collision.rigidbody')
  - [transform](#F-gdio-common-objects-Collision-transform 'gdio.common.objects.Collision.transform')
- [Color](#T-gdio-common-objects-Color 'gdio.common.objects.Color')
  - [a](#F-gdio-common-objects-Color-a 'gdio.common.objects.Color.a')
  - [b](#F-gdio-common-objects-Color-b 'gdio.common.objects.Color.b')
  - [g](#F-gdio-common-objects-Color-g 'gdio.common.objects.Color.g')
  - [r](#F-gdio-common-objects-Color-r 'gdio.common.objects.Color.r')
- [CoordinateConversion](#T-gdio-common-objects-CoordinateConversion 'gdio.common.objects.CoordinateConversion')
  - [Local](#F-gdio-common-objects-CoordinateConversion-Local 'gdio.common.objects.CoordinateConversion.Local')
  - [None](#F-gdio-common-objects-CoordinateConversion-None 'gdio.common.objects.CoordinateConversion.None')
  - [ScreenToViewportPoint](#F-gdio-common-objects-CoordinateConversion-ScreenToViewportPoint 'gdio.common.objects.CoordinateConversion.ScreenToViewportPoint')
  - [ScreenToWorldPoint](#F-gdio-common-objects-CoordinateConversion-ScreenToWorldPoint 'gdio.common.objects.CoordinateConversion.ScreenToWorldPoint')
  - [ViewportToScreenPoint](#F-gdio-common-objects-CoordinateConversion-ViewportToScreenPoint 'gdio.common.objects.CoordinateConversion.ViewportToScreenPoint')
  - [ViewportToWorldPoint](#F-gdio-common-objects-CoordinateConversion-ViewportToWorldPoint 'gdio.common.objects.CoordinateConversion.ViewportToWorldPoint')
  - [WorldToScreenPoint](#F-gdio-common-objects-CoordinateConversion-WorldToScreenPoint 'gdio.common.objects.CoordinateConversion.WorldToScreenPoint')
  - [WorldToViewportPoint](#F-gdio-common-objects-CoordinateConversion-WorldToViewportPoint 'gdio.common.objects.CoordinateConversion.WorldToViewportPoint')
- [GameConnectionDetails](#T-gdio-common-objects-GameConnectionDetails 'gdio.common.objects.GameConnectionDetails')
  - [Addr](#F-gdio-common-objects-GameConnectionDetails-Addr 'gdio.common.objects.GameConnectionDetails.Addr')
  - [GamePath](#F-gdio-common-objects-GameConnectionDetails-GamePath 'gdio.common.objects.GameConnectionDetails.GamePath')
  - [IsEditor](#F-gdio-common-objects-GameConnectionDetails-IsEditor 'gdio.common.objects.GameConnectionDetails.IsEditor')
  - [Platform](#F-gdio-common-objects-GameConnectionDetails-Platform 'gdio.common.objects.GameConnectionDetails.Platform')
  - [Port](#F-gdio-common-objects-GameConnectionDetails-Port 'gdio.common.objects.GameConnectionDetails.Port')
- [LiteComponent](#T-gdio-common-objects-LiteComponent 'gdio.common.objects.LiteComponent')
  - [gameObject](#F-gdio-common-objects-LiteComponent-gameObject 'gdio.common.objects.LiteComponent.gameObject')
  - [hierarchyPath](#F-gdio-common-objects-LiteComponent-hierarchyPath 'gdio.common.objects.LiteComponent.hierarchyPath')
  - [tag](#F-gdio-common-objects-LiteComponent-tag 'gdio.common.objects.LiteComponent.tag')
  - [transform](#F-gdio-common-objects-LiteComponent-transform 'gdio.common.objects.LiteComponent.transform')
  - [typeFullName](#F-gdio-common-objects-LiteComponent-typeFullName 'gdio.common.objects.LiteComponent.typeFullName')
- [LiteGameObject](#T-gdio-common-objects-LiteGameObject 'gdio.common.objects.LiteGameObject')
  - [Components](#F-gdio-common-objects-LiteGameObject-Components 'gdio.common.objects.LiteGameObject.Components')
  - [activeSelf](#F-gdio-common-objects-LiteGameObject-activeSelf 'gdio.common.objects.LiteGameObject.activeSelf')
  - [hashCode](#F-gdio-common-objects-LiteGameObject-hashCode 'gdio.common.objects.LiteGameObject.hashCode')
  - [hierarchyPath](#F-gdio-common-objects-LiteGameObject-hierarchyPath 'gdio.common.objects.LiteGameObject.hierarchyPath')
  - [localPosition](#F-gdio-common-objects-LiteGameObject-localPosition 'gdio.common.objects.LiteGameObject.localPosition')
  - [parentHashCode](#F-gdio-common-objects-LiteGameObject-parentHashCode 'gdio.common.objects.LiteGameObject.parentHashCode')
  - [position](#F-gdio-common-objects-LiteGameObject-position 'gdio.common.objects.LiteGameObject.position')
  - [rotation](#F-gdio-common-objects-LiteGameObject-rotation 'gdio.common.objects.LiteGameObject.rotation')
  - [sceneId](#F-gdio-common-objects-LiteGameObject-sceneId 'gdio.common.objects.LiteGameObject.sceneId')
  - [sceneName](#F-gdio-common-objects-LiteGameObject-sceneName 'gdio.common.objects.LiteGameObject.sceneName')
  - [scenePath](#F-gdio-common-objects-LiteGameObject-scenePath 'gdio.common.objects.LiteGameObject.scenePath')
  - [tag](#F-gdio-common-objects-LiteGameObject-tag 'gdio.common.objects.LiteGameObject.tag')
  - [transform](#F-gdio-common-objects-LiteGameObject-transform 'gdio.common.objects.LiteGameObject.transform')
  - [typeFullName](#F-gdio-common-objects-LiteGameObject-typeFullName 'gdio.common.objects.LiteGameObject.typeFullName')
- [LiteObject](#T-gdio-common-objects-LiteObject 'gdio.common.objects.LiteObject')
  - [instanceId](#F-gdio-common-objects-LiteObject-instanceId 'gdio.common.objects.LiteObject.instanceId')
  - [name](#F-gdio-common-objects-LiteObject-name 'gdio.common.objects.LiteObject.name')
- [Matrix4x4](#T-gdio-common-objects-Matrix4x4 'gdio.common.objects.Matrix4x4')
- [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons')
  - [LEFT](#F-gdio-common-objects-MouseButtons-LEFT 'gdio.common.objects.MouseButtons.LEFT')
  - [MIDDLE](#F-gdio-common-objects-MouseButtons-MIDDLE 'gdio.common.objects.MouseButtons.MIDDLE')
  - [RIGHT](#F-gdio-common-objects-MouseButtons-RIGHT 'gdio.common.objects.MouseButtons.RIGHT')
- [ObjectListFilter](#T-gdio-common-objects-ObjectListFilter 'gdio.common.objects.ObjectListFilter')
  - [ALL](#F-gdio-common-objects-ObjectListFilter-ALL 'gdio.common.objects.ObjectListFilter.ALL')
  - [TAGGED](#F-gdio-common-objects-ObjectListFilter-TAGGED 'gdio.common.objects.ObjectListFilter.TAGGED')
  - [UNTAGGED](#F-gdio-common-objects-ObjectListFilter-UNTAGGED 'gdio.common.objects.ObjectListFilter.UNTAGGED')
- [PhysicMaterial](#T-gdio-common-objects-PhysicMaterial 'gdio.common.objects.PhysicMaterial')
  - [bounceCombine](#F-gdio-common-objects-PhysicMaterial-bounceCombine 'gdio.common.objects.PhysicMaterial.bounceCombine')
  - [bounciness](#F-gdio-common-objects-PhysicMaterial-bounciness 'gdio.common.objects.PhysicMaterial.bounciness')
  - [dynamicFriction](#F-gdio-common-objects-PhysicMaterial-dynamicFriction 'gdio.common.objects.PhysicMaterial.dynamicFriction')
  - [frictionCombine](#F-gdio-common-objects-PhysicMaterial-frictionCombine 'gdio.common.objects.PhysicMaterial.frictionCombine')
  - [staticFriction](#F-gdio-common-objects-PhysicMaterial-staticFriction 'gdio.common.objects.PhysicMaterial.staticFriction')
- [Quaternion](#T-gdio-common-objects-Quaternion 'gdio.common.objects.Quaternion')
  - [w](#F-gdio-common-objects-Quaternion-w 'gdio.common.objects.Quaternion.w')
  - [x](#F-gdio-common-objects-Quaternion-x 'gdio.common.objects.Quaternion.x')
  - [y](#F-gdio-common-objects-Quaternion-y 'gdio.common.objects.Quaternion.y')
  - [z](#F-gdio-common-objects-Quaternion-z 'gdio.common.objects.Quaternion.z')
- [RaycastResult](#T-gdio-common-objects-RaycastResult 'gdio.common.objects.RaycastResult')
  - [hasButton](#P-gdio-common-objects-RaycastResult-hasButton 'gdio.common.objects.RaycastResult.hasButton')
  - [name](#P-gdio-common-objects-RaycastResult-name 'gdio.common.objects.RaycastResult.name')
  - [point](#P-gdio-common-objects-RaycastResult-point 'gdio.common.objects.RaycastResult.point')
  - [tag](#P-gdio-common-objects-RaycastResult-tag 'gdio.common.objects.RaycastResult.tag')
  - [type](#P-gdio-common-objects-RaycastResult-type 'gdio.common.objects.RaycastResult.type')
  - [typeFullName](#P-gdio-common-objects-RaycastResult-typeFullName 'gdio.common.objects.RaycastResult.typeFullName')
- [Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space')
  - [Self](#F-gdio-common-objects-Space-Self 'gdio.common.objects.Space.Self')
  - [World](#F-gdio-common-objects-Space-World 'gdio.common.objects.Space.World')
- [Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2')
  - [x](#F-gdio-common-objects-Vector2-x 'gdio.common.objects.Vector2.x')
  - [y](#F-gdio-common-objects-Vector2-y 'gdio.common.objects.Vector2.y')
- [Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3')
  - [x](#F-gdio-common-objects-Vector3-x 'gdio.common.objects.Vector3.x')
  - [y](#F-gdio-common-objects-Vector3-y 'gdio.common.objects.Vector3.y')
  - [z](#F-gdio-common-objects-Vector3-z 'gdio.common.objects.Vector3.z')
- [Vector4](#T-gdio-common-objects-Vector4 'gdio.common.objects.Vector4')
  - [w](#F-gdio-common-objects-Vector4-w 'gdio.common.objects.Vector4.w')
  - [x](#F-gdio-common-objects-Vector4-x 'gdio.common.objects.Vector4.x')
  - [y](#F-gdio-common-objects-Vector4-y 'gdio.common.objects.Vector4.y')
  - [z](#F-gdio-common-objects-Vector4-z 'gdio.common.objects.Vector4.z')

<a name='T-gdio-common-objects-COLLISION_EVENT'></a>
## COLLISION_EVENT `type`

##### Namespace

gdio.common.objects

##### Summary

The type of collision event received.

<a name='F-gdio-common-objects-COLLISION_EVENT-COLLISION_ENTER'></a>
### COLLISION_ENTER `constants`

##### Summary

Colliding object has entered the collision bounds.

<a name='F-gdio-common-objects-COLLISION_EVENT-COLLISION_EXIT'></a>
### COLLISION_EXIT `constants`

##### Summary

Colliding object exited collision bounds.

<a name='F-gdio-common-objects-COLLISION_EVENT-COLLISION_STAY'></a>
### COLLISION_STAY `constants`

##### Summary

Colliding object still loated in the collision bounds

<a name='T-gdio-common-objects-Collider'></a>
## Collider `type`

##### Namespace

gdio.common.objects

##### Summary

The lite version of the [UnityEngine.Collider](https://docs.unity3d.com/ScriptReference/Collider.html)

<a name='F-gdio-common-objects-Collider-attachedRigidbody'></a>
### attachedRigidbody `constants`

##### Summary

The [Rigidbody](#T-gdio-common-objects-Rigidbody 'gdio.common.objects.Rigidbody') that the collider is attached to.

<a name='F-gdio-common-objects-Collider-bounds'></a>
### bounds `constants`

##### Summary

The [Bounds](#T-gdio-common-objects-Bounds 'gdio.common.objects.Bounds') of the collider.

<a name='F-gdio-common-objects-Collider-contactOffset'></a>
### contactOffset `constants`

##### Summary

Contact offset value of the collider.

<a name='F-gdio-common-objects-Collider-enabled'></a>
### enabled `constants`

##### Summary

Boolean if the collider is enabled or not.

<a name='F-gdio-common-objects-Collider-isTrigger'></a>
### isTrigger `constants`

##### Summary

Boolean if the collider is a trigger or not.

<a name='F-gdio-common-objects-Collider-material'></a>
### material `constants`

##### Summary

The [PhysicMaterial](#T-gdio-common-objects-PhysicMaterial 'gdio.common.objects.PhysicMaterial') of the collider.

<a name='F-gdio-common-objects-Collider-sharedMaterial'></a>
### sharedMaterial `constants`

##### Summary

The shared [PhysicMaterial](#T-gdio-common-objects-PhysicMaterial 'gdio.common.objects.PhysicMaterial') of the collider.

<a name='T-gdio-common-objects-Collision'></a>
## Collision `type`

##### Namespace

gdio.common.objects

##### Summary

Describes a collision.

<a name='F-gdio-common-objects-Collision-CollisionType'></a>
### CollisionType `constants`

##### Summary

The enumeration value of the collision type [COLLISION_EVENT](#T-gdio-common-objects-COLLISION_EVENT 'gdio.common.objects.COLLISION_EVENT')

<a name='F-gdio-common-objects-Collision-HierarchyPath'></a>
### HierarchyPath `constants`

##### Summary

The [HierarchyPath](https://support.gamedriver.io/support/solutions/articles/69000385849-working-with-hierarchypath) of the GameObject that received the OnCollision event.

<a name='F-gdio-common-objects-Collision-Timestamp'></a>
### Timestamp `constants`

##### Summary

The timestamp of when the collision occurred.

<a name='F-gdio-common-objects-Collision-contactCount'></a>
### contactCount `constants`

##### Summary

The number of contacts in the collision.

<a name='F-gdio-common-objects-Collision-contacts'></a>
### contacts `constants`

##### Summary

Array of contacts, [ContactPoint](#T-gdio-common-objects-ContactPoint 'gdio.common.objects.ContactPoint')

<a name='F-gdio-common-objects-Collision-gameObject'></a>
### gameObject `constants`

##### Summary

The [LiteGameObject](#T-gdio-common-objects-LiteGameObject 'gdio.common.objects.LiteGameObject') of the collision.

<a name='F-gdio-common-objects-Collision-impulse'></a>
### impulse `constants`

##### Summary

A [Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') describing the impulse value.

<a name='F-gdio-common-objects-Collision-relativeVelocity'></a>
### relativeVelocity `constants`

##### Summary

A [Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') describing the relative velocity value.

<a name='F-gdio-common-objects-Collision-rigidbody'></a>
### rigidbody `constants`

##### Summary

The [Rigidbody](#T-gdio-common-objects-Rigidbody 'gdio.common.objects.Rigidbody') of the collision.

<a name='F-gdio-common-objects-Collision-transform'></a>
### transform `constants`

##### Summary

The [Transform](#T-gdio-common-objects-Transform 'gdio.common.objects.Transform') of the GameObject.

<a name='T-gdio-common-objects-Color'></a>
## Color `type`

##### Namespace

gdio.common.objects

##### Summary

A numerical representation of Color.

<a name='F-gdio-common-objects-Color-a'></a>
### a `constants`

##### Summary

The alpha (transparency) value.

<a name='F-gdio-common-objects-Color-b'></a>
### b `constants`

##### Summary

The blue value.

<a name='F-gdio-common-objects-Color-g'></a>
### g `constants`

##### Summary

The green value.

<a name='F-gdio-common-objects-Color-r'></a>
### r `constants`

##### Summary

The red value.

<a name='T-gdio-common-objects-CoordinateConversion'></a>
## CoordinateConversion `type`

##### Namespace

gdio.common.objects

##### Summary

Enumeration for the type of coordinate conversion.

<a name='F-gdio-common-objects-CoordinateConversion-Local'></a>
### Local `constants`

##### Summary

Local returns the [GameObject.Transform.localPosition](https://docs.unity3d.com/ScriptReference/Transform-localPosition.html) without any conversion.

<a name='F-gdio-common-objects-CoordinateConversion-None'></a>
### None `constants`

##### Summary

None returns the [GameObject.Transform.position](https://docs.unity3d.com/ScriptReference/Transform-position.html) without any conversion.

<a name='F-gdio-common-objects-CoordinateConversion-ScreenToViewportPoint'></a>
### ScreenToViewportPoint `constants`

##### Summary

ScreenToViewPortPoint returns the coordinates of the object in the viewport space of the specified Camera. The default is [Camera.main](https://docs.unity3d.com/ScriptReference/Camera-main.html).

<a name='F-gdio-common-objects-CoordinateConversion-ScreenToWorldPoint'></a>
### ScreenToWorldPoint `constants`

##### Summary

ScreenToWorldPoint returns the coordinates of the object in the world space of the specified Camera. The default is [Camera.main](https://docs.unity3d.com/ScriptReference/Camera-main.html).

<a name='F-gdio-common-objects-CoordinateConversion-ViewportToScreenPoint'></a>
### ViewportToScreenPoint `constants`

##### Summary

ScreenToViewPortPoint returns the coordinates of the object in the viewport space of the specified Camera. The default is [Camera.main](https://docs.unity3d.com/ScriptReference/Camera-main.html).

<a name='F-gdio-common-objects-CoordinateConversion-ViewportToWorldPoint'></a>
### ViewportToWorldPoint `constants`

##### Summary

ScreenToWorldPoint returns the coordinates of the object in the world space of the specified Camera. The default is [Camera.main](https://docs.unity3d.com/ScriptReference/Camera-main.html).

<a name='F-gdio-common-objects-CoordinateConversion-WorldToScreenPoint'></a>
### WorldToScreenPoint `constants`

##### Summary

WorldToScreenPoint returns the coordinates of the object transformed from World-To-Screen by the specified Camera. The default is [Camera.main](https://docs.unity3d.com/ScriptReference/Camera-main.html).

<a name='F-gdio-common-objects-CoordinateConversion-WorldToViewportPoint'></a>
### WorldToViewportPoint `constants`

##### Summary

WorldToViewPortPoint returns the coordinates of the object in the screen space of the specified Camera. The default is [Camera.main](https://docs.unity3d.com/ScriptReference/Camera-main.html).

<a name='T-gdio-common-objects-GameConnectionDetails'></a>
## GameConnectionDetails `type`

##### Namespace

gdio.common.objects

##### Summary

This class provides information about the currently connected game.

<a name='F-gdio-common-objects-GameConnectionDetails-Addr'></a>
### Addr `constants`

##### Summary

The [IPAddress](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Net.IPAddress 'System.Net.IPAddress') of the connected game.

<a name='F-gdio-common-objects-GameConnectionDetails-GamePath'></a>
### GamePath `constants`

##### Summary

The [Application.dataPath](https://docs.unity3d.com/ScriptReference/Application-dataPath.html) of the connected game.

<a name='F-gdio-common-objects-GameConnectionDetails-IsEditor'></a>
### IsEditor `constants`

##### Summary

Boolean value if the game is running in an Unity editor instance.

<a name='F-gdio-common-objects-GameConnectionDetails-Platform'></a>
### Platform `constants`

##### Summary

The [Application.platform](https://docs.unity3d.com/ScriptReference/Application-platform.html) of the connected game.

<a name='F-gdio-common-objects-GameConnectionDetails-Port'></a>
### Port `constants`

##### Summary

The port number of the connected game.

<a name='T-gdio-common-objects-LiteComponent'></a>
## LiteComponent `type`

##### Namespace

gdio.common.objects

##### Summary

A simplistic version of [UnityEngine.Component](https://docs.unity3d.com/ScriptReference/Component.html)

<a name='F-gdio-common-objects-LiteComponent-gameObject'></a>
### gameObject `constants`

##### Summary

The lite version of the [GameObject](https://docs.unity3d.com/ScriptReference/GameObject.html) the component is attached to.

<a name='F-gdio-common-objects-LiteComponent-hierarchyPath'></a>
### hierarchyPath `constants`

##### Summary

The [HierarchyPath](https://support.gamedriver.io/support/solutions/articles/69000385849-working-with-hierarchypath) of the component.

<a name='F-gdio-common-objects-LiteComponent-tag'></a>
### tag `constants`

##### Summary

The tag of the [GameObject](https://docs.unity3d.com/ScriptReference/GameObject.html).

<a name='F-gdio-common-objects-LiteComponent-transform'></a>
### transform `constants`

##### Summary

The transform attached to the [GameObject](https://docs.unity3d.com/ScriptReference/GameObject.html).

<a name='F-gdio-common-objects-LiteComponent-typeFullName'></a>
### typeFullName `constants`

##### Summary

The Type fullname of the class.

<a name='T-gdio-common-objects-LiteGameObject'></a>
## LiteGameObject `type`

##### Namespace

gdio.common.objects

##### Summary

This is a lite version of the [GameObject](https://docs.unity3d.com/ScriptReference/GameObject.html).

<a name='F-gdio-common-objects-LiteGameObject-Components'></a>
### Components `constants`

##### Summary

A list of the Component Types associated with the object.

<a name='F-gdio-common-objects-LiteGameObject-activeSelf'></a>
### activeSelf `constants`

##### Summary

A boolean indicating whether the object is active in the scene.

<a name='F-gdio-common-objects-LiteGameObject-hashCode'></a>
### hashCode `constants`

##### Summary

The Hash Code of the object.

<a name='F-gdio-common-objects-LiteGameObject-hierarchyPath'></a>
### hierarchyPath `constants`

##### Summary

The [HierarchyPath](https://support.gamedriver.io/support/solutions/articles/69000385849-working-with-hierarchypath) to the GameObject.

<a name='F-gdio-common-objects-LiteGameObject-localPosition'></a>
### localPosition `constants`

##### Summary

The Local Position of the object.

<a name='F-gdio-common-objects-LiteGameObject-parentHashCode'></a>
### parentHashCode `constants`

##### Summary

The Hash Code of the Parent object.

<a name='F-gdio-common-objects-LiteGameObject-position'></a>
### position `constants`

##### Summary

The Absolute Position of the object.

<a name='F-gdio-common-objects-LiteGameObject-rotation'></a>
### rotation `constants`

##### Summary

The Rotation of the object.

<a name='F-gdio-common-objects-LiteGameObject-sceneId'></a>
### sceneId `constants`

##### Summary

The Scene ID.

<a name='F-gdio-common-objects-LiteGameObject-sceneName'></a>
### sceneName `constants`

##### Summary

The Name of the Scene.

<a name='F-gdio-common-objects-LiteGameObject-scenePath'></a>
### scenePath `constants`

##### Summary

The Path of the Scene.

<a name='F-gdio-common-objects-LiteGameObject-tag'></a>
### tag `constants`

##### Summary

The Tag of the object.

<a name='F-gdio-common-objects-LiteGameObject-transform'></a>
### transform `constants`

##### Summary

Position, rotation, and scale of the object.

<a name='F-gdio-common-objects-LiteGameObject-typeFullName'></a>
### typeFullName `constants`

##### Summary

The Full Type the object.

<a name='T-gdio-common-objects-LiteObject'></a>
## LiteObject `type`

##### Namespace

gdio.common.objects

##### Summary

A simplistic version of [UnityEngine.GameObject](https://docs.unity3d.com/ScriptReference/GameObject.html)

<a name='F-gdio-common-objects-LiteObject-instanceId'></a>
### instanceId `constants`

##### Summary

The instanceId of the object.

<a name='F-gdio-common-objects-LiteObject-name'></a>
### name `constants`

##### Summary

The name of the object.

<a name='T-gdio-common-objects-Matrix4x4'></a>
## Matrix4x4 `type`

##### Namespace

gdio.common.objects

##### Summary

A standard 4x4 transformation matrix.

<a name='T-gdio-common-objects-MouseButtons'></a>
## MouseButtons `type`

##### Namespace

gdio.common.objects

##### Summary

Mouse button enumerations to use for input.

<a name='F-gdio-common-objects-MouseButtons-LEFT'></a>
### LEFT `constants`

##### Summary

Left Mouse Button

<a name='F-gdio-common-objects-MouseButtons-MIDDLE'></a>
### MIDDLE `constants`

##### Summary

Middle Mouse Button

<a name='F-gdio-common-objects-MouseButtons-RIGHT'></a>
### RIGHT `constants`

##### Summary

Right Mouse Button

<a name='T-gdio-common-objects-ObjectListFilter'></a>
## ObjectListFilter `type`

##### Namespace

gdio.common.objects

##### Summary

Enumeration to filter objects by.

<a name='F-gdio-common-objects-ObjectListFilter-ALL'></a>
### ALL `constants`

##### Summary

All objects, returns tagged and untagged object list

<a name='F-gdio-common-objects-ObjectListFilter-TAGGED'></a>
### TAGGED `constants`

##### Summary

TAGGED objects, returns their tag

<a name='F-gdio-common-objects-ObjectListFilter-UNTAGGED'></a>
### UNTAGGED `constants`

##### Summary

Untagged objects, returns their name

<a name='T-gdio-common-objects-PhysicMaterial'></a>
## PhysicMaterial `type`

##### Namespace

gdio.common.objects

##### Summary

Physics material describes how to handle collisions.

<a name='F-gdio-common-objects-PhysicMaterial-bounceCombine'></a>
### bounceCombine `constants`

##### Summary

Determines how the bounciness is combined. (Unity 2018)

<a name='F-gdio-common-objects-PhysicMaterial-bounciness'></a>
### bounciness `constants`

##### Summary

How bouncy a surface is.

<a name='F-gdio-common-objects-PhysicMaterial-dynamicFriction'></a>
### dynamicFriction `constants`

##### Summary

The friction used when already moving.

<a name='F-gdio-common-objects-PhysicMaterial-frictionCombine'></a>
### frictionCombine `constants`

##### Summary

Determines how the friction is combined. (Unity 2018)

<a name='F-gdio-common-objects-PhysicMaterial-staticFriction'></a>
### staticFriction `constants`

##### Summary

The friction coefficient used when an object is lying on the surface.

<a name='T-gdio-common-objects-Quaternion'></a>
## Quaternion `type`

##### Namespace

gdio.common.objects

##### Summary

A mathematical representation of 3D rotation. See [here](#!-https-//scriptinghelpers-org/blog/how-to-think-about-quaternions 'https://scriptinghelpers.org/blog/how-to-think-about-quaternions') for more information.


<a name='F-gdio-common-objects-Quaternion-w'></a>
### w `constants`

##### Summary

The w component.

<a name='F-gdio-common-objects-Quaternion-x'></a>
### x `constants`

##### Summary

The x component.

<a name='F-gdio-common-objects-Quaternion-y'></a>
### y `constants`

##### Summary

The y component.

<a name='F-gdio-common-objects-Quaternion-z'></a>
### z `constants`

##### Summary

The x component.

<a name='T-gdio-common-objects-RaycastResult'></a>
## RaycastResult `type`

##### Namespace

gdio.common.objects

##### Summary

Structure used to get information back from a raycast. Used for visual objects only.

<a name='P-gdio-common-objects-RaycastResult-hasButton'></a>
### hasButton `property`

##### Summary

Boolean of whether the object hit by the raycast has a Button component.

<a name='P-gdio-common-objects-RaycastResult-name'></a>
### name `property`

##### Summary

The Name of the object hit by the raycast.

<a name='P-gdio-common-objects-RaycastResult-point'></a>
### point `property`

##### Summary

The impact point in world space where the ray hit the collider.

<a name='P-gdio-common-objects-RaycastResult-tag'></a>
### tag `property`

##### Summary

The Tag of the object hit by the raycast.

<a name='P-gdio-common-objects-RaycastResult-type'></a>
### type `property`

##### Summary

The Type of object hit by the raycase (e.g. Physics).

<a name='P-gdio-common-objects-RaycastResult-typeFullName'></a>
### typeFullName `property`

##### Summary

The name of the object class (e.g. [UnityEngine.GameObject](https://docs.unity3d.com/ScriptReference/GameObject.html))

<a name='T-gdio-common-objects-Space'></a>
## Space `type`

##### Namespace

gdio.common.objects

##### Summary

Enumeration of the Space type.

<a name='F-gdio-common-objects-Space-Self'></a>
### Self `constants`

##### Summary

The Self Space enumeration.

<a name='F-gdio-common-objects-Space-World'></a>
### World `constants`

##### Summary

The World Space enumeration.

<a name='T-gdio-common-objects-Vector2'></a>
## Vector2 `type`

##### Namespace

gdio.common.objects

##### Summary

A representation of 2D vectors and points.

<a name='F-gdio-common-objects-Vector2-x'></a>
### x `constants`

##### Summary

The x component.

<a name='F-gdio-common-objects-Vector2-y'></a>
### y `constants`

##### Summary

The y component.

<a name='T-gdio-common-objects-Vector3'></a>
## Vector3 `type`

##### Namespace

gdio.common.objects

##### Summary

A representation of 3D vectors and points.

<a name='F-gdio-common-objects-Vector3-x'></a>
### x `constants`

##### Summary

The x coordinate of the position.

<a name='F-gdio-common-objects-Vector3-y'></a>
### y `constants`

##### Summary

The y coordinate of the position.

<a name='F-gdio-common-objects-Vector3-z'></a>
### z `constants`

##### Summary

The z coordinate of the position.

<a name='T-gdio-common-objects-Vector4'></a>
## Vector4 `type`

##### Namespace

gdio.common.objects

##### Summary

A representation of 3D vectors and points.

<a name='F-gdio-common-objects-Vector4-w'></a>
### w `constants`

##### Summary

The w component.

<a name='F-gdio-common-objects-Vector4-x'></a>
### x `constants`

##### Summary

The x component.

<a name='F-gdio-common-objects-Vector4-y'></a>
### y `constants`

##### Summary

The y component.

<a name='F-gdio-common-objects-Vector4-z'></a>
### z `constants`

##### Summary

The z component.

