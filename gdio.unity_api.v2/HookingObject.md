# HookingObject enumeration

Enumeration of input types that can be hooked. Currently TOUCHINPUT is bundled with MOUSE and GAMEPAD is not supported.

```csharp
public enum HookingObject
```

## Values

| name | value | description |
| --- | --- | --- |
| KEYBOARD | `1` | Keyboard input |
| MOUSE | `2` | Mouse input |
| GAMEPAD | `4` | Gamepad input, CURRENTLY NOT SUPPORTED |
| TOUCHINPUT | `8` | Touch input, enum value is currently not used. Enabled/Disabled via MOUSE enumeration. |
| ALL | `15` | All inputs |

## See Also

* namespace [gdio.unity_api.v2](../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->