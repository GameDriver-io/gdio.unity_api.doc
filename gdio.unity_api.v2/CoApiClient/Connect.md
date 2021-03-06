# CoApiClient.Connect method (1 of 2)

Use this function to connect to a Unity game with GameDriver Agent configured and active. This function can connect to only the UnityEditor, and must be used within the Unity Test Runner.

```csharp
public IEnumerator<bool> Connect()
```

## See Also

* class [CoApiClient](../CoApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

---

# CoApiClient.Connect method (2 of 2)

Use this function to connect to a Unity game with GameDriver Agent configured and active. This function can connect to the UnityEditor or a Standalone deployment of a game.

```csharp
public IEnumerator<bool> Connect(string hostname, int port = 19734, int timeout = 30)
```

| parameter | description |
| --- | --- |
| hostname | The hostname of the machine running the game. |
| port | The configured port that the GameDriver agent is configured to use. |
| timeout | The amount of time in seconds to wait for connectivity to establish with the game. |

## See Also

* class [CoApiClient](../CoApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
