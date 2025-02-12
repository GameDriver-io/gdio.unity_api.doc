# ApiClient.CreateObjectRef method (1 of 3)

Create an ObjectRef using an hpath.

```csharp
public ObjectRef CreateObjectRef(string hpath, int timeout = 30)
```

| parameter | description |
| --- | --- |
| hpath | HiearchyPath of the object to store the refernce |
| timeout | Timeout in seconds |

## Return Value

ObjectRef

## Exceptions

| exception | condition |
| --- | --- |
| Exception | Failed to create the Object |

## Examples

```csharp
var sliderPath = "//*[@name='ActiveSlider']/fn:component('UnityEngine.UI.Slider')";
var sliderRef = api.CreateObjectRef(hpath:sliderPath);
// usage in hpath queries
var val = api.GetObjectFieldValue<float>($"fn:objectref('{sliderRef}')/@value");
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

---

# ApiClient.CreateObjectRef method (2 of 3)

Instantiate an Object (Not a GameObject) using its full type name and Constructor params if any

```csharp
public ObjectRef CreateObjectRef(string type, object[] arguments = null, int timeout = 30)
```

| parameter | description |
| --- | --- |
| type | Full Type name of the object |
| arguments | Constructor params if any |
| timeout | Timeout in seconds |

## Return Value

`ObjectRef` to the object

## Examples

```csharp
// Say the game has an EnemyModel(string name, int resistance) class that backs enemy info and you need to
// instantiate an object of it in a test, CreateObjectRef does just that 
var enemyModelRef = api.CreateObjectRef("SomeNamespace.EnemyModel", new object[] { "SwampMonster", 9 });
// Do something that changes any properties of the object
// direct access
var enemyResistance = api.GetObjectFieldValue<int>(enemyModelRef, "Resistance");
// access from within hpath queries
var enemyResistance = api.GetObjectFieldValue<int>($"fn:objectref('{enemyModelRef}')/@Resistance");
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

---

# ApiClient.CreateObjectRef method (3 of 3)

Instantiate an Object (Not a GameObject) using its `Type` and Constructor params if any and store it's reference as an ObjectRef.

```csharp
public ObjectRef CreateObjectRef(Type type, object[] arguments = null, int timeout = 30)
```

| parameter | description |
| --- | --- |
| type | Type of the object |
| arguments | Constructor params if any |
| timeout | Timeout in seconds |

## Return Value

`ObjectRef` to the object

## Examples

```csharp
// Say the game has an EnemyModel(string name, int resistance) class that backs enemy info and you need to
// instantiate an object of it in a test, CreateObjectRef does just that 
var enemyModelRef = api.CreateObjectRef(typeof(SomeNamespace.EnemyModel), new object[] { "SwampMonster", 9 }); // If you have access to the type from the test script.
// Do something that changes any properties of the object
// direct access
var enemyResistance = api.GetObjectFieldValue<int>(enemyModelRef, "Resistance");
// access from within hpath queries
var enemyResistance = api.GetObjectFieldValue<int>($"fn:objectref('{enemyModelRef}')/@Resistance");
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
