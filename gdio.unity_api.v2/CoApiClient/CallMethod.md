# CoApiClient.CallMethod method (1 of 2)

Use this function to execute a [System.Void](https://learn.microsoft.com/en-us/dotnet/api/system.void) method on an object or from a static class.

```csharp
public IEnumerator<bool> CallMethod(string hierarchyPath, string methodName, 
    object[] arguments = null, int timeout = 30)
```

| parameter | description |
| --- | --- |
| hierarchyPath | The HierarchyPath for the object that the script component is attached to or the static class. |
| methodName | The name of the method to call. |
| arguments | An array of objects to pass as arguments to the method. |
| timeout | The number of seconds to wait for a response that the request was processed. |

## Return Value

Returns a boolean based on the successful execution of the return type void method.

## Examples

```csharp
api.CallMethod("//*[@name='Canvas']/fn:component('CustomScript')",
                "CustomMethod", new string[] { "string:The Test was run on " + DateTime.Now.ToShortDateString() });
            
            //CallMethod can even be used to pass HPathObjects without the need for custom serialization.
            api.CallMethod("//*[@name='HPathDataObject']/fn:component('HPathObjectScript')",
                "HPathObjectMethod", new object[] { new HPathObject("//*[@name='ObjectHPathRef']") });
```

## See Also

* class [CoApiClient](../CoApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

---

# CoApiClient.CallMethod&lt;T&gt; method (2 of 2)

Use this function to execute a method on an object.

```csharp
public IEnumerator<T> CallMethod<T>(string hierarchyPath, string methodName, object[] arguments, 
    int timeout = 30)
```

| parameter | description |
| --- | --- |
| hierarchyPath | The HierarchyPath for the object that the script component is attached to. |
| methodName | The name of the method to call. |
| arguments | An array of objects to pass as arguments to the method. |
| timeout | The number of seconds to wait for a response that the request was processed. |

## Return Value

Returns a deserialized object of type T. If T and the type of the returned object don't match, an exception will be thrown.

## Examples

```csharp
api.CallMethod<int>("//*[@name='Canvas']/fn:component('CustomScript')", "DoMath", new object[] { 1, 2 });
```

## See Also

* class [CoApiClient](../CoApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
