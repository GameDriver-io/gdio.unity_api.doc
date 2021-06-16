<a name='assembly'></a>
# ENUMS

## Contents

- [GDI32](#T-gdio-unity_api-utilities-ScreenCapture-GDI32 'gdio.unity_api.utilities.ScreenCapture.GDI32')
- [GameConnectionDetails](#T-gdio-unity_api-v2-GameConnectionDetails 'gdio.unity_api.v2.GameConnectionDetails')
  - [Addr](#F-gdio-unity_api-v2-GameConnectionDetails-Addr 'gdio.unity_api.v2.GameConnectionDetails.Addr')
  - [GamePath](#F-gdio-unity_api-v2-GameConnectionDetails-GamePath 'gdio.unity_api.v2.GameConnectionDetails.GamePath')
  - [IsEditor](#F-gdio-unity_api-v2-GameConnectionDetails-IsEditor 'gdio.unity_api.v2.GameConnectionDetails.IsEditor')
  - [IsStandalone](#F-gdio-unity_api-v2-GameConnectionDetails-IsStandalone 'gdio.unity_api.v2.GameConnectionDetails.IsStandalone')
  - [Platform](#F-gdio-unity_api-v2-GameConnectionDetails-Platform 'gdio.unity_api.v2.GameConnectionDetails.Platform')
  - [Port](#F-gdio-unity_api-v2-GameConnectionDetails-Port 'gdio.unity_api.v2.GameConnectionDetails.Port')
- [HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject')
  - [ALL](#F-gdio-unity_api-v2-HookingObject-ALL 'gdio.unity_api.v2.HookingObject.ALL')
  - [GAMEPAD](#F-gdio-unity_api-v2-HookingObject-GAMEPAD 'gdio.unity_api.v2.HookingObject.GAMEPAD')
  - [KEYBOARD](#F-gdio-unity_api-v2-HookingObject-KEYBOARD 'gdio.unity_api.v2.HookingObject.KEYBOARD')
  - [MOUSE](#F-gdio-unity_api-v2-HookingObject-MOUSE 'gdio.unity_api.v2.HookingObject.MOUSE')
  - [TOUCHINPUT](#F-gdio-unity_api-v2-HookingObject-TOUCHINPUT 'gdio.unity_api.v2.HookingObject.TOUCHINPUT')
- [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode')
  - [A](#F-gdio-unity_api-KeyCode-A 'gdio.unity_api.KeyCode.A')
  - [Alpha0](#F-gdio-unity_api-KeyCode-Alpha0 'gdio.unity_api.KeyCode.Alpha0')
  - [Alpha1](#F-gdio-unity_api-KeyCode-Alpha1 'gdio.unity_api.KeyCode.Alpha1')
  - [Alpha2](#F-gdio-unity_api-KeyCode-Alpha2 'gdio.unity_api.KeyCode.Alpha2')
  - [Alpha3](#F-gdio-unity_api-KeyCode-Alpha3 'gdio.unity_api.KeyCode.Alpha3')
  - [Alpha4](#F-gdio-unity_api-KeyCode-Alpha4 'gdio.unity_api.KeyCode.Alpha4')
  - [Alpha5](#F-gdio-unity_api-KeyCode-Alpha5 'gdio.unity_api.KeyCode.Alpha5')
  - [Alpha6](#F-gdio-unity_api-KeyCode-Alpha6 'gdio.unity_api.KeyCode.Alpha6')
  - [Alpha7](#F-gdio-unity_api-KeyCode-Alpha7 'gdio.unity_api.KeyCode.Alpha7')
  - [Alpha8](#F-gdio-unity_api-KeyCode-Alpha8 'gdio.unity_api.KeyCode.Alpha8')
  - [Alpha9](#F-gdio-unity_api-KeyCode-Alpha9 'gdio.unity_api.KeyCode.Alpha9')
  - [AltGr](#F-gdio-unity_api-KeyCode-AltGr 'gdio.unity_api.KeyCode.AltGr')
  - [Ampersand](#F-gdio-unity_api-KeyCode-Ampersand 'gdio.unity_api.KeyCode.Ampersand')
  - [Asterisk](#F-gdio-unity_api-KeyCode-Asterisk 'gdio.unity_api.KeyCode.Asterisk')
  - [At](#F-gdio-unity_api-KeyCode-At 'gdio.unity_api.KeyCode.At')
  - [B](#F-gdio-unity_api-KeyCode-B 'gdio.unity_api.KeyCode.B')
  - [BackQuote](#F-gdio-unity_api-KeyCode-BackQuote 'gdio.unity_api.KeyCode.BackQuote')
  - [Backslash](#F-gdio-unity_api-KeyCode-Backslash 'gdio.unity_api.KeyCode.Backslash')
  - [Backspace](#F-gdio-unity_api-KeyCode-Backspace 'gdio.unity_api.KeyCode.Backspace')
  - [Break](#F-gdio-unity_api-KeyCode-Break 'gdio.unity_api.KeyCode.Break')
  - [C](#F-gdio-unity_api-KeyCode-C 'gdio.unity_api.KeyCode.C')
  - [CapsLock](#F-gdio-unity_api-KeyCode-CapsLock 'gdio.unity_api.KeyCode.CapsLock')
  - [Caret](#F-gdio-unity_api-KeyCode-Caret 'gdio.unity_api.KeyCode.Caret')
  - [Clear](#F-gdio-unity_api-KeyCode-Clear 'gdio.unity_api.KeyCode.Clear')
  - [Colon](#F-gdio-unity_api-KeyCode-Colon 'gdio.unity_api.KeyCode.Colon')
  - [Comma](#F-gdio-unity_api-KeyCode-Comma 'gdio.unity_api.KeyCode.Comma')
  - [D](#F-gdio-unity_api-KeyCode-D 'gdio.unity_api.KeyCode.D')
  - [Delete](#F-gdio-unity_api-KeyCode-Delete 'gdio.unity_api.KeyCode.Delete')
  - [Dollar](#F-gdio-unity_api-KeyCode-Dollar 'gdio.unity_api.KeyCode.Dollar')
  - [DoubleQuote](#F-gdio-unity_api-KeyCode-DoubleQuote 'gdio.unity_api.KeyCode.DoubleQuote')
  - [DownArrow](#F-gdio-unity_api-KeyCode-DownArrow 'gdio.unity_api.KeyCode.DownArrow')
  - [E](#F-gdio-unity_api-KeyCode-E 'gdio.unity_api.KeyCode.E')
  - [End](#F-gdio-unity_api-KeyCode-End 'gdio.unity_api.KeyCode.End')
  - [Equals](#F-gdio-unity_api-KeyCode-Equals 'gdio.unity_api.KeyCode.Equals')
  - [Escape](#F-gdio-unity_api-KeyCode-Escape 'gdio.unity_api.KeyCode.Escape')
  - [Exclaim](#F-gdio-unity_api-KeyCode-Exclaim 'gdio.unity_api.KeyCode.Exclaim')
  - [F](#F-gdio-unity_api-KeyCode-F 'gdio.unity_api.KeyCode.F')
  - [F1](#F-gdio-unity_api-KeyCode-F1 'gdio.unity_api.KeyCode.F1')
  - [F10](#F-gdio-unity_api-KeyCode-F10 'gdio.unity_api.KeyCode.F10')
  - [F11](#F-gdio-unity_api-KeyCode-F11 'gdio.unity_api.KeyCode.F11')
  - [F12](#F-gdio-unity_api-KeyCode-F12 'gdio.unity_api.KeyCode.F12')
  - [F13](#F-gdio-unity_api-KeyCode-F13 'gdio.unity_api.KeyCode.F13')
  - [F14](#F-gdio-unity_api-KeyCode-F14 'gdio.unity_api.KeyCode.F14')
  - [F15](#F-gdio-unity_api-KeyCode-F15 'gdio.unity_api.KeyCode.F15')
  - [F2](#F-gdio-unity_api-KeyCode-F2 'gdio.unity_api.KeyCode.F2')
  - [F3](#F-gdio-unity_api-KeyCode-F3 'gdio.unity_api.KeyCode.F3')
  - [F4](#F-gdio-unity_api-KeyCode-F4 'gdio.unity_api.KeyCode.F4')
  - [F5](#F-gdio-unity_api-KeyCode-F5 'gdio.unity_api.KeyCode.F5')
  - [F6](#F-gdio-unity_api-KeyCode-F6 'gdio.unity_api.KeyCode.F6')
  - [F7](#F-gdio-unity_api-KeyCode-F7 'gdio.unity_api.KeyCode.F7')
  - [F8](#F-gdio-unity_api-KeyCode-F8 'gdio.unity_api.KeyCode.F8')
  - [F9](#F-gdio-unity_api-KeyCode-F9 'gdio.unity_api.KeyCode.F9')
  - [G](#F-gdio-unity_api-KeyCode-G 'gdio.unity_api.KeyCode.G')
  - [Greater](#F-gdio-unity_api-KeyCode-Greater 'gdio.unity_api.KeyCode.Greater')
  - [H](#F-gdio-unity_api-KeyCode-H 'gdio.unity_api.KeyCode.H')
  - [Hash](#F-gdio-unity_api-KeyCode-Hash 'gdio.unity_api.KeyCode.Hash')
  - [Help](#F-gdio-unity_api-KeyCode-Help 'gdio.unity_api.KeyCode.Help')
  - [Home](#F-gdio-unity_api-KeyCode-Home 'gdio.unity_api.KeyCode.Home')
  - [I](#F-gdio-unity_api-KeyCode-I 'gdio.unity_api.KeyCode.I')
  - [Insert](#F-gdio-unity_api-KeyCode-Insert 'gdio.unity_api.KeyCode.Insert')
  - [J](#F-gdio-unity_api-KeyCode-J 'gdio.unity_api.KeyCode.J')
  - [Joystick1Button0](#F-gdio-unity_api-KeyCode-Joystick1Button0 'gdio.unity_api.KeyCode.Joystick1Button0')
  - [Joystick1Button1](#F-gdio-unity_api-KeyCode-Joystick1Button1 'gdio.unity_api.KeyCode.Joystick1Button1')
  - [Joystick1Button10](#F-gdio-unity_api-KeyCode-Joystick1Button10 'gdio.unity_api.KeyCode.Joystick1Button10')
  - [Joystick1Button11](#F-gdio-unity_api-KeyCode-Joystick1Button11 'gdio.unity_api.KeyCode.Joystick1Button11')
  - [Joystick1Button12](#F-gdio-unity_api-KeyCode-Joystick1Button12 'gdio.unity_api.KeyCode.Joystick1Button12')
  - [Joystick1Button13](#F-gdio-unity_api-KeyCode-Joystick1Button13 'gdio.unity_api.KeyCode.Joystick1Button13')
  - [Joystick1Button14](#F-gdio-unity_api-KeyCode-Joystick1Button14 'gdio.unity_api.KeyCode.Joystick1Button14')
  - [Joystick1Button15](#F-gdio-unity_api-KeyCode-Joystick1Button15 'gdio.unity_api.KeyCode.Joystick1Button15')
  - [Joystick1Button16](#F-gdio-unity_api-KeyCode-Joystick1Button16 'gdio.unity_api.KeyCode.Joystick1Button16')
  - [Joystick1Button17](#F-gdio-unity_api-KeyCode-Joystick1Button17 'gdio.unity_api.KeyCode.Joystick1Button17')
  - [Joystick1Button18](#F-gdio-unity_api-KeyCode-Joystick1Button18 'gdio.unity_api.KeyCode.Joystick1Button18')
  - [Joystick1Button19](#F-gdio-unity_api-KeyCode-Joystick1Button19 'gdio.unity_api.KeyCode.Joystick1Button19')
  - [Joystick1Button2](#F-gdio-unity_api-KeyCode-Joystick1Button2 'gdio.unity_api.KeyCode.Joystick1Button2')
  - [Joystick1Button3](#F-gdio-unity_api-KeyCode-Joystick1Button3 'gdio.unity_api.KeyCode.Joystick1Button3')
  - [Joystick1Button4](#F-gdio-unity_api-KeyCode-Joystick1Button4 'gdio.unity_api.KeyCode.Joystick1Button4')
  - [Joystick1Button5](#F-gdio-unity_api-KeyCode-Joystick1Button5 'gdio.unity_api.KeyCode.Joystick1Button5')
  - [Joystick1Button6](#F-gdio-unity_api-KeyCode-Joystick1Button6 'gdio.unity_api.KeyCode.Joystick1Button6')
  - [Joystick1Button7](#F-gdio-unity_api-KeyCode-Joystick1Button7 'gdio.unity_api.KeyCode.Joystick1Button7')
  - [Joystick1Button8](#F-gdio-unity_api-KeyCode-Joystick1Button8 'gdio.unity_api.KeyCode.Joystick1Button8')
  - [Joystick1Button9](#F-gdio-unity_api-KeyCode-Joystick1Button9 'gdio.unity_api.KeyCode.Joystick1Button9')
  - [Joystick2Button0](#F-gdio-unity_api-KeyCode-Joystick2Button0 'gdio.unity_api.KeyCode.Joystick2Button0')
  - [Joystick2Button1](#F-gdio-unity_api-KeyCode-Joystick2Button1 'gdio.unity_api.KeyCode.Joystick2Button1')
  - [Joystick2Button10](#F-gdio-unity_api-KeyCode-Joystick2Button10 'gdio.unity_api.KeyCode.Joystick2Button10')
  - [Joystick2Button11](#F-gdio-unity_api-KeyCode-Joystick2Button11 'gdio.unity_api.KeyCode.Joystick2Button11')
  - [Joystick2Button12](#F-gdio-unity_api-KeyCode-Joystick2Button12 'gdio.unity_api.KeyCode.Joystick2Button12')
  - [Joystick2Button13](#F-gdio-unity_api-KeyCode-Joystick2Button13 'gdio.unity_api.KeyCode.Joystick2Button13')
  - [Joystick2Button14](#F-gdio-unity_api-KeyCode-Joystick2Button14 'gdio.unity_api.KeyCode.Joystick2Button14')
  - [Joystick2Button15](#F-gdio-unity_api-KeyCode-Joystick2Button15 'gdio.unity_api.KeyCode.Joystick2Button15')
  - [Joystick2Button16](#F-gdio-unity_api-KeyCode-Joystick2Button16 'gdio.unity_api.KeyCode.Joystick2Button16')
  - [Joystick2Button17](#F-gdio-unity_api-KeyCode-Joystick2Button17 'gdio.unity_api.KeyCode.Joystick2Button17')
  - [Joystick2Button18](#F-gdio-unity_api-KeyCode-Joystick2Button18 'gdio.unity_api.KeyCode.Joystick2Button18')
  - [Joystick2Button19](#F-gdio-unity_api-KeyCode-Joystick2Button19 'gdio.unity_api.KeyCode.Joystick2Button19')
  - [Joystick2Button2](#F-gdio-unity_api-KeyCode-Joystick2Button2 'gdio.unity_api.KeyCode.Joystick2Button2')
  - [Joystick2Button3](#F-gdio-unity_api-KeyCode-Joystick2Button3 'gdio.unity_api.KeyCode.Joystick2Button3')
  - [Joystick2Button4](#F-gdio-unity_api-KeyCode-Joystick2Button4 'gdio.unity_api.KeyCode.Joystick2Button4')
  - [Joystick2Button5](#F-gdio-unity_api-KeyCode-Joystick2Button5 'gdio.unity_api.KeyCode.Joystick2Button5')
  - [Joystick2Button6](#F-gdio-unity_api-KeyCode-Joystick2Button6 'gdio.unity_api.KeyCode.Joystick2Button6')
  - [Joystick2Button7](#F-gdio-unity_api-KeyCode-Joystick2Button7 'gdio.unity_api.KeyCode.Joystick2Button7')
  - [Joystick2Button8](#F-gdio-unity_api-KeyCode-Joystick2Button8 'gdio.unity_api.KeyCode.Joystick2Button8')
  - [Joystick2Button9](#F-gdio-unity_api-KeyCode-Joystick2Button9 'gdio.unity_api.KeyCode.Joystick2Button9')
  - [Joystick3Button0](#F-gdio-unity_api-KeyCode-Joystick3Button0 'gdio.unity_api.KeyCode.Joystick3Button0')
  - [Joystick3Button1](#F-gdio-unity_api-KeyCode-Joystick3Button1 'gdio.unity_api.KeyCode.Joystick3Button1')
  - [Joystick3Button10](#F-gdio-unity_api-KeyCode-Joystick3Button10 'gdio.unity_api.KeyCode.Joystick3Button10')
  - [Joystick3Button11](#F-gdio-unity_api-KeyCode-Joystick3Button11 'gdio.unity_api.KeyCode.Joystick3Button11')
  - [Joystick3Button12](#F-gdio-unity_api-KeyCode-Joystick3Button12 'gdio.unity_api.KeyCode.Joystick3Button12')
  - [Joystick3Button13](#F-gdio-unity_api-KeyCode-Joystick3Button13 'gdio.unity_api.KeyCode.Joystick3Button13')
  - [Joystick3Button14](#F-gdio-unity_api-KeyCode-Joystick3Button14 'gdio.unity_api.KeyCode.Joystick3Button14')
  - [Joystick3Button15](#F-gdio-unity_api-KeyCode-Joystick3Button15 'gdio.unity_api.KeyCode.Joystick3Button15')
  - [Joystick3Button16](#F-gdio-unity_api-KeyCode-Joystick3Button16 'gdio.unity_api.KeyCode.Joystick3Button16')
  - [Joystick3Button17](#F-gdio-unity_api-KeyCode-Joystick3Button17 'gdio.unity_api.KeyCode.Joystick3Button17')
  - [Joystick3Button18](#F-gdio-unity_api-KeyCode-Joystick3Button18 'gdio.unity_api.KeyCode.Joystick3Button18')
  - [Joystick3Button19](#F-gdio-unity_api-KeyCode-Joystick3Button19 'gdio.unity_api.KeyCode.Joystick3Button19')
  - [Joystick3Button2](#F-gdio-unity_api-KeyCode-Joystick3Button2 'gdio.unity_api.KeyCode.Joystick3Button2')
  - [Joystick3Button3](#F-gdio-unity_api-KeyCode-Joystick3Button3 'gdio.unity_api.KeyCode.Joystick3Button3')
  - [Joystick3Button4](#F-gdio-unity_api-KeyCode-Joystick3Button4 'gdio.unity_api.KeyCode.Joystick3Button4')
  - [Joystick3Button5](#F-gdio-unity_api-KeyCode-Joystick3Button5 'gdio.unity_api.KeyCode.Joystick3Button5')
  - [Joystick3Button6](#F-gdio-unity_api-KeyCode-Joystick3Button6 'gdio.unity_api.KeyCode.Joystick3Button6')
  - [Joystick3Button7](#F-gdio-unity_api-KeyCode-Joystick3Button7 'gdio.unity_api.KeyCode.Joystick3Button7')
  - [Joystick3Button8](#F-gdio-unity_api-KeyCode-Joystick3Button8 'gdio.unity_api.KeyCode.Joystick3Button8')
  - [Joystick3Button9](#F-gdio-unity_api-KeyCode-Joystick3Button9 'gdio.unity_api.KeyCode.Joystick3Button9')
  - [Joystick4Button0](#F-gdio-unity_api-KeyCode-Joystick4Button0 'gdio.unity_api.KeyCode.Joystick4Button0')
  - [Joystick4Button1](#F-gdio-unity_api-KeyCode-Joystick4Button1 'gdio.unity_api.KeyCode.Joystick4Button1')
  - [Joystick4Button10](#F-gdio-unity_api-KeyCode-Joystick4Button10 'gdio.unity_api.KeyCode.Joystick4Button10')
  - [Joystick4Button11](#F-gdio-unity_api-KeyCode-Joystick4Button11 'gdio.unity_api.KeyCode.Joystick4Button11')
  - [Joystick4Button12](#F-gdio-unity_api-KeyCode-Joystick4Button12 'gdio.unity_api.KeyCode.Joystick4Button12')
  - [Joystick4Button13](#F-gdio-unity_api-KeyCode-Joystick4Button13 'gdio.unity_api.KeyCode.Joystick4Button13')
  - [Joystick4Button14](#F-gdio-unity_api-KeyCode-Joystick4Button14 'gdio.unity_api.KeyCode.Joystick4Button14')
  - [Joystick4Button15](#F-gdio-unity_api-KeyCode-Joystick4Button15 'gdio.unity_api.KeyCode.Joystick4Button15')
  - [Joystick4Button16](#F-gdio-unity_api-KeyCode-Joystick4Button16 'gdio.unity_api.KeyCode.Joystick4Button16')
  - [Joystick4Button17](#F-gdio-unity_api-KeyCode-Joystick4Button17 'gdio.unity_api.KeyCode.Joystick4Button17')
  - [Joystick4Button18](#F-gdio-unity_api-KeyCode-Joystick4Button18 'gdio.unity_api.KeyCode.Joystick4Button18')
  - [Joystick4Button19](#F-gdio-unity_api-KeyCode-Joystick4Button19 'gdio.unity_api.KeyCode.Joystick4Button19')
  - [Joystick4Button2](#F-gdio-unity_api-KeyCode-Joystick4Button2 'gdio.unity_api.KeyCode.Joystick4Button2')
  - [Joystick4Button3](#F-gdio-unity_api-KeyCode-Joystick4Button3 'gdio.unity_api.KeyCode.Joystick4Button3')
  - [Joystick4Button4](#F-gdio-unity_api-KeyCode-Joystick4Button4 'gdio.unity_api.KeyCode.Joystick4Button4')
  - [Joystick4Button5](#F-gdio-unity_api-KeyCode-Joystick4Button5 'gdio.unity_api.KeyCode.Joystick4Button5')
  - [Joystick4Button6](#F-gdio-unity_api-KeyCode-Joystick4Button6 'gdio.unity_api.KeyCode.Joystick4Button6')
  - [Joystick4Button7](#F-gdio-unity_api-KeyCode-Joystick4Button7 'gdio.unity_api.KeyCode.Joystick4Button7')
  - [Joystick4Button8](#F-gdio-unity_api-KeyCode-Joystick4Button8 'gdio.unity_api.KeyCode.Joystick4Button8')
  - [Joystick4Button9](#F-gdio-unity_api-KeyCode-Joystick4Button9 'gdio.unity_api.KeyCode.Joystick4Button9')
  - [Joystick5Button0](#F-gdio-unity_api-KeyCode-Joystick5Button0 'gdio.unity_api.KeyCode.Joystick5Button0')
  - [Joystick5Button1](#F-gdio-unity_api-KeyCode-Joystick5Button1 'gdio.unity_api.KeyCode.Joystick5Button1')
  - [Joystick5Button10](#F-gdio-unity_api-KeyCode-Joystick5Button10 'gdio.unity_api.KeyCode.Joystick5Button10')
  - [Joystick5Button11](#F-gdio-unity_api-KeyCode-Joystick5Button11 'gdio.unity_api.KeyCode.Joystick5Button11')
  - [Joystick5Button12](#F-gdio-unity_api-KeyCode-Joystick5Button12 'gdio.unity_api.KeyCode.Joystick5Button12')
  - [Joystick5Button13](#F-gdio-unity_api-KeyCode-Joystick5Button13 'gdio.unity_api.KeyCode.Joystick5Button13')
  - [Joystick5Button14](#F-gdio-unity_api-KeyCode-Joystick5Button14 'gdio.unity_api.KeyCode.Joystick5Button14')
  - [Joystick5Button15](#F-gdio-unity_api-KeyCode-Joystick5Button15 'gdio.unity_api.KeyCode.Joystick5Button15')
  - [Joystick5Button16](#F-gdio-unity_api-KeyCode-Joystick5Button16 'gdio.unity_api.KeyCode.Joystick5Button16')
  - [Joystick5Button17](#F-gdio-unity_api-KeyCode-Joystick5Button17 'gdio.unity_api.KeyCode.Joystick5Button17')
  - [Joystick5Button18](#F-gdio-unity_api-KeyCode-Joystick5Button18 'gdio.unity_api.KeyCode.Joystick5Button18')
  - [Joystick5Button19](#F-gdio-unity_api-KeyCode-Joystick5Button19 'gdio.unity_api.KeyCode.Joystick5Button19')
  - [Joystick5Button2](#F-gdio-unity_api-KeyCode-Joystick5Button2 'gdio.unity_api.KeyCode.Joystick5Button2')
  - [Joystick5Button3](#F-gdio-unity_api-KeyCode-Joystick5Button3 'gdio.unity_api.KeyCode.Joystick5Button3')
  - [Joystick5Button4](#F-gdio-unity_api-KeyCode-Joystick5Button4 'gdio.unity_api.KeyCode.Joystick5Button4')
  - [Joystick5Button5](#F-gdio-unity_api-KeyCode-Joystick5Button5 'gdio.unity_api.KeyCode.Joystick5Button5')
  - [Joystick5Button6](#F-gdio-unity_api-KeyCode-Joystick5Button6 'gdio.unity_api.KeyCode.Joystick5Button6')
  - [Joystick5Button7](#F-gdio-unity_api-KeyCode-Joystick5Button7 'gdio.unity_api.KeyCode.Joystick5Button7')
  - [Joystick5Button8](#F-gdio-unity_api-KeyCode-Joystick5Button8 'gdio.unity_api.KeyCode.Joystick5Button8')
  - [Joystick5Button9](#F-gdio-unity_api-KeyCode-Joystick5Button9 'gdio.unity_api.KeyCode.Joystick5Button9')
  - [Joystick6Button0](#F-gdio-unity_api-KeyCode-Joystick6Button0 'gdio.unity_api.KeyCode.Joystick6Button0')
  - [Joystick6Button1](#F-gdio-unity_api-KeyCode-Joystick6Button1 'gdio.unity_api.KeyCode.Joystick6Button1')
  - [Joystick6Button10](#F-gdio-unity_api-KeyCode-Joystick6Button10 'gdio.unity_api.KeyCode.Joystick6Button10')
  - [Joystick6Button11](#F-gdio-unity_api-KeyCode-Joystick6Button11 'gdio.unity_api.KeyCode.Joystick6Button11')
  - [Joystick6Button12](#F-gdio-unity_api-KeyCode-Joystick6Button12 'gdio.unity_api.KeyCode.Joystick6Button12')
  - [Joystick6Button13](#F-gdio-unity_api-KeyCode-Joystick6Button13 'gdio.unity_api.KeyCode.Joystick6Button13')
  - [Joystick6Button14](#F-gdio-unity_api-KeyCode-Joystick6Button14 'gdio.unity_api.KeyCode.Joystick6Button14')
  - [Joystick6Button15](#F-gdio-unity_api-KeyCode-Joystick6Button15 'gdio.unity_api.KeyCode.Joystick6Button15')
  - [Joystick6Button16](#F-gdio-unity_api-KeyCode-Joystick6Button16 'gdio.unity_api.KeyCode.Joystick6Button16')
  - [Joystick6Button17](#F-gdio-unity_api-KeyCode-Joystick6Button17 'gdio.unity_api.KeyCode.Joystick6Button17')
  - [Joystick6Button18](#F-gdio-unity_api-KeyCode-Joystick6Button18 'gdio.unity_api.KeyCode.Joystick6Button18')
  - [Joystick6Button19](#F-gdio-unity_api-KeyCode-Joystick6Button19 'gdio.unity_api.KeyCode.Joystick6Button19')
  - [Joystick6Button2](#F-gdio-unity_api-KeyCode-Joystick6Button2 'gdio.unity_api.KeyCode.Joystick6Button2')
  - [Joystick6Button3](#F-gdio-unity_api-KeyCode-Joystick6Button3 'gdio.unity_api.KeyCode.Joystick6Button3')
  - [Joystick6Button4](#F-gdio-unity_api-KeyCode-Joystick6Button4 'gdio.unity_api.KeyCode.Joystick6Button4')
  - [Joystick6Button5](#F-gdio-unity_api-KeyCode-Joystick6Button5 'gdio.unity_api.KeyCode.Joystick6Button5')
  - [Joystick6Button6](#F-gdio-unity_api-KeyCode-Joystick6Button6 'gdio.unity_api.KeyCode.Joystick6Button6')
  - [Joystick6Button7](#F-gdio-unity_api-KeyCode-Joystick6Button7 'gdio.unity_api.KeyCode.Joystick6Button7')
  - [Joystick6Button8](#F-gdio-unity_api-KeyCode-Joystick6Button8 'gdio.unity_api.KeyCode.Joystick6Button8')
  - [Joystick6Button9](#F-gdio-unity_api-KeyCode-Joystick6Button9 'gdio.unity_api.KeyCode.Joystick6Button9')
  - [Joystick7Button0](#F-gdio-unity_api-KeyCode-Joystick7Button0 'gdio.unity_api.KeyCode.Joystick7Button0')
  - [Joystick7Button1](#F-gdio-unity_api-KeyCode-Joystick7Button1 'gdio.unity_api.KeyCode.Joystick7Button1')
  - [Joystick7Button10](#F-gdio-unity_api-KeyCode-Joystick7Button10 'gdio.unity_api.KeyCode.Joystick7Button10')
  - [Joystick7Button11](#F-gdio-unity_api-KeyCode-Joystick7Button11 'gdio.unity_api.KeyCode.Joystick7Button11')
  - [Joystick7Button12](#F-gdio-unity_api-KeyCode-Joystick7Button12 'gdio.unity_api.KeyCode.Joystick7Button12')
  - [Joystick7Button13](#F-gdio-unity_api-KeyCode-Joystick7Button13 'gdio.unity_api.KeyCode.Joystick7Button13')
  - [Joystick7Button14](#F-gdio-unity_api-KeyCode-Joystick7Button14 'gdio.unity_api.KeyCode.Joystick7Button14')
  - [Joystick7Button15](#F-gdio-unity_api-KeyCode-Joystick7Button15 'gdio.unity_api.KeyCode.Joystick7Button15')
  - [Joystick7Button16](#F-gdio-unity_api-KeyCode-Joystick7Button16 'gdio.unity_api.KeyCode.Joystick7Button16')
  - [Joystick7Button17](#F-gdio-unity_api-KeyCode-Joystick7Button17 'gdio.unity_api.KeyCode.Joystick7Button17')
  - [Joystick7Button18](#F-gdio-unity_api-KeyCode-Joystick7Button18 'gdio.unity_api.KeyCode.Joystick7Button18')
  - [Joystick7Button19](#F-gdio-unity_api-KeyCode-Joystick7Button19 'gdio.unity_api.KeyCode.Joystick7Button19')
  - [Joystick7Button2](#F-gdio-unity_api-KeyCode-Joystick7Button2 'gdio.unity_api.KeyCode.Joystick7Button2')
  - [Joystick7Button3](#F-gdio-unity_api-KeyCode-Joystick7Button3 'gdio.unity_api.KeyCode.Joystick7Button3')
  - [Joystick7Button4](#F-gdio-unity_api-KeyCode-Joystick7Button4 'gdio.unity_api.KeyCode.Joystick7Button4')
  - [Joystick7Button5](#F-gdio-unity_api-KeyCode-Joystick7Button5 'gdio.unity_api.KeyCode.Joystick7Button5')
  - [Joystick7Button6](#F-gdio-unity_api-KeyCode-Joystick7Button6 'gdio.unity_api.KeyCode.Joystick7Button6')
  - [Joystick7Button7](#F-gdio-unity_api-KeyCode-Joystick7Button7 'gdio.unity_api.KeyCode.Joystick7Button7')
  - [Joystick7Button8](#F-gdio-unity_api-KeyCode-Joystick7Button8 'gdio.unity_api.KeyCode.Joystick7Button8')
  - [Joystick7Button9](#F-gdio-unity_api-KeyCode-Joystick7Button9 'gdio.unity_api.KeyCode.Joystick7Button9')
  - [Joystick8Button0](#F-gdio-unity_api-KeyCode-Joystick8Button0 'gdio.unity_api.KeyCode.Joystick8Button0')
  - [Joystick8Button1](#F-gdio-unity_api-KeyCode-Joystick8Button1 'gdio.unity_api.KeyCode.Joystick8Button1')
  - [Joystick8Button10](#F-gdio-unity_api-KeyCode-Joystick8Button10 'gdio.unity_api.KeyCode.Joystick8Button10')
  - [Joystick8Button11](#F-gdio-unity_api-KeyCode-Joystick8Button11 'gdio.unity_api.KeyCode.Joystick8Button11')
  - [Joystick8Button12](#F-gdio-unity_api-KeyCode-Joystick8Button12 'gdio.unity_api.KeyCode.Joystick8Button12')
  - [Joystick8Button13](#F-gdio-unity_api-KeyCode-Joystick8Button13 'gdio.unity_api.KeyCode.Joystick8Button13')
  - [Joystick8Button14](#F-gdio-unity_api-KeyCode-Joystick8Button14 'gdio.unity_api.KeyCode.Joystick8Button14')
  - [Joystick8Button15](#F-gdio-unity_api-KeyCode-Joystick8Button15 'gdio.unity_api.KeyCode.Joystick8Button15')
  - [Joystick8Button16](#F-gdio-unity_api-KeyCode-Joystick8Button16 'gdio.unity_api.KeyCode.Joystick8Button16')
  - [Joystick8Button17](#F-gdio-unity_api-KeyCode-Joystick8Button17 'gdio.unity_api.KeyCode.Joystick8Button17')
  - [Joystick8Button18](#F-gdio-unity_api-KeyCode-Joystick8Button18 'gdio.unity_api.KeyCode.Joystick8Button18')
  - [Joystick8Button19](#F-gdio-unity_api-KeyCode-Joystick8Button19 'gdio.unity_api.KeyCode.Joystick8Button19')
  - [Joystick8Button2](#F-gdio-unity_api-KeyCode-Joystick8Button2 'gdio.unity_api.KeyCode.Joystick8Button2')
  - [Joystick8Button3](#F-gdio-unity_api-KeyCode-Joystick8Button3 'gdio.unity_api.KeyCode.Joystick8Button3')
  - [Joystick8Button4](#F-gdio-unity_api-KeyCode-Joystick8Button4 'gdio.unity_api.KeyCode.Joystick8Button4')
  - [Joystick8Button5](#F-gdio-unity_api-KeyCode-Joystick8Button5 'gdio.unity_api.KeyCode.Joystick8Button5')
  - [Joystick8Button6](#F-gdio-unity_api-KeyCode-Joystick8Button6 'gdio.unity_api.KeyCode.Joystick8Button6')
  - [Joystick8Button7](#F-gdio-unity_api-KeyCode-Joystick8Button7 'gdio.unity_api.KeyCode.Joystick8Button7')
  - [Joystick8Button8](#F-gdio-unity_api-KeyCode-Joystick8Button8 'gdio.unity_api.KeyCode.Joystick8Button8')
  - [Joystick8Button9](#F-gdio-unity_api-KeyCode-Joystick8Button9 'gdio.unity_api.KeyCode.Joystick8Button9')
  - [JoystickButton0](#F-gdio-unity_api-KeyCode-JoystickButton0 'gdio.unity_api.KeyCode.JoystickButton0')
  - [JoystickButton1](#F-gdio-unity_api-KeyCode-JoystickButton1 'gdio.unity_api.KeyCode.JoystickButton1')
  - [JoystickButton10](#F-gdio-unity_api-KeyCode-JoystickButton10 'gdio.unity_api.KeyCode.JoystickButton10')
  - [JoystickButton11](#F-gdio-unity_api-KeyCode-JoystickButton11 'gdio.unity_api.KeyCode.JoystickButton11')
  - [JoystickButton12](#F-gdio-unity_api-KeyCode-JoystickButton12 'gdio.unity_api.KeyCode.JoystickButton12')
  - [JoystickButton13](#F-gdio-unity_api-KeyCode-JoystickButton13 'gdio.unity_api.KeyCode.JoystickButton13')
  - [JoystickButton14](#F-gdio-unity_api-KeyCode-JoystickButton14 'gdio.unity_api.KeyCode.JoystickButton14')
  - [JoystickButton15](#F-gdio-unity_api-KeyCode-JoystickButton15 'gdio.unity_api.KeyCode.JoystickButton15')
  - [JoystickButton16](#F-gdio-unity_api-KeyCode-JoystickButton16 'gdio.unity_api.KeyCode.JoystickButton16')
  - [JoystickButton17](#F-gdio-unity_api-KeyCode-JoystickButton17 'gdio.unity_api.KeyCode.JoystickButton17')
  - [JoystickButton18](#F-gdio-unity_api-KeyCode-JoystickButton18 'gdio.unity_api.KeyCode.JoystickButton18')
  - [JoystickButton19](#F-gdio-unity_api-KeyCode-JoystickButton19 'gdio.unity_api.KeyCode.JoystickButton19')
  - [JoystickButton2](#F-gdio-unity_api-KeyCode-JoystickButton2 'gdio.unity_api.KeyCode.JoystickButton2')
  - [JoystickButton3](#F-gdio-unity_api-KeyCode-JoystickButton3 'gdio.unity_api.KeyCode.JoystickButton3')
  - [JoystickButton4](#F-gdio-unity_api-KeyCode-JoystickButton4 'gdio.unity_api.KeyCode.JoystickButton4')
  - [JoystickButton5](#F-gdio-unity_api-KeyCode-JoystickButton5 'gdio.unity_api.KeyCode.JoystickButton5')
  - [JoystickButton6](#F-gdio-unity_api-KeyCode-JoystickButton6 'gdio.unity_api.KeyCode.JoystickButton6')
  - [JoystickButton7](#F-gdio-unity_api-KeyCode-JoystickButton7 'gdio.unity_api.KeyCode.JoystickButton7')
  - [JoystickButton8](#F-gdio-unity_api-KeyCode-JoystickButton8 'gdio.unity_api.KeyCode.JoystickButton8')
  - [JoystickButton9](#F-gdio-unity_api-KeyCode-JoystickButton9 'gdio.unity_api.KeyCode.JoystickButton9')
  - [K](#F-gdio-unity_api-KeyCode-K 'gdio.unity_api.KeyCode.K')
  - [Keypad0](#F-gdio-unity_api-KeyCode-Keypad0 'gdio.unity_api.KeyCode.Keypad0')
  - [Keypad1](#F-gdio-unity_api-KeyCode-Keypad1 'gdio.unity_api.KeyCode.Keypad1')
  - [Keypad2](#F-gdio-unity_api-KeyCode-Keypad2 'gdio.unity_api.KeyCode.Keypad2')
  - [Keypad3](#F-gdio-unity_api-KeyCode-Keypad3 'gdio.unity_api.KeyCode.Keypad3')
  - [Keypad4](#F-gdio-unity_api-KeyCode-Keypad4 'gdio.unity_api.KeyCode.Keypad4')
  - [Keypad5](#F-gdio-unity_api-KeyCode-Keypad5 'gdio.unity_api.KeyCode.Keypad5')
  - [Keypad6](#F-gdio-unity_api-KeyCode-Keypad6 'gdio.unity_api.KeyCode.Keypad6')
  - [Keypad7](#F-gdio-unity_api-KeyCode-Keypad7 'gdio.unity_api.KeyCode.Keypad7')
  - [Keypad8](#F-gdio-unity_api-KeyCode-Keypad8 'gdio.unity_api.KeyCode.Keypad8')
  - [Keypad9](#F-gdio-unity_api-KeyCode-Keypad9 'gdio.unity_api.KeyCode.Keypad9')
  - [KeypadDivide](#F-gdio-unity_api-KeyCode-KeypadDivide 'gdio.unity_api.KeyCode.KeypadDivide')
  - [KeypadEnter](#F-gdio-unity_api-KeyCode-KeypadEnter 'gdio.unity_api.KeyCode.KeypadEnter')
  - [KeypadEquals](#F-gdio-unity_api-KeyCode-KeypadEquals 'gdio.unity_api.KeyCode.KeypadEquals')
  - [KeypadMinus](#F-gdio-unity_api-KeyCode-KeypadMinus 'gdio.unity_api.KeyCode.KeypadMinus')
  - [KeypadMultiply](#F-gdio-unity_api-KeyCode-KeypadMultiply 'gdio.unity_api.KeyCode.KeypadMultiply')
  - [KeypadPeriod](#F-gdio-unity_api-KeyCode-KeypadPeriod 'gdio.unity_api.KeyCode.KeypadPeriod')
  - [KeypadPlus](#F-gdio-unity_api-KeyCode-KeypadPlus 'gdio.unity_api.KeyCode.KeypadPlus')
  - [L](#F-gdio-unity_api-KeyCode-L 'gdio.unity_api.KeyCode.L')
  - [LeftAlt](#F-gdio-unity_api-KeyCode-LeftAlt 'gdio.unity_api.KeyCode.LeftAlt')
  - [LeftApple](#F-gdio-unity_api-KeyCode-LeftApple 'gdio.unity_api.KeyCode.LeftApple')
  - [LeftArrow](#F-gdio-unity_api-KeyCode-LeftArrow 'gdio.unity_api.KeyCode.LeftArrow')
  - [LeftBracket](#F-gdio-unity_api-KeyCode-LeftBracket 'gdio.unity_api.KeyCode.LeftBracket')
  - [LeftCommand](#F-gdio-unity_api-KeyCode-LeftCommand 'gdio.unity_api.KeyCode.LeftCommand')
  - [LeftControl](#F-gdio-unity_api-KeyCode-LeftControl 'gdio.unity_api.KeyCode.LeftControl')
  - [LeftParen](#F-gdio-unity_api-KeyCode-LeftParen 'gdio.unity_api.KeyCode.LeftParen')
  - [LeftShift](#F-gdio-unity_api-KeyCode-LeftShift 'gdio.unity_api.KeyCode.LeftShift')
  - [LeftWindows](#F-gdio-unity_api-KeyCode-LeftWindows 'gdio.unity_api.KeyCode.LeftWindows')
  - [Less](#F-gdio-unity_api-KeyCode-Less 'gdio.unity_api.KeyCode.Less')
  - [M](#F-gdio-unity_api-KeyCode-M 'gdio.unity_api.KeyCode.M')
  - [Menu](#F-gdio-unity_api-KeyCode-Menu 'gdio.unity_api.KeyCode.Menu')
  - [Minus](#F-gdio-unity_api-KeyCode-Minus 'gdio.unity_api.KeyCode.Minus')
  - [Mouse0](#F-gdio-unity_api-KeyCode-Mouse0 'gdio.unity_api.KeyCode.Mouse0')
  - [Mouse1](#F-gdio-unity_api-KeyCode-Mouse1 'gdio.unity_api.KeyCode.Mouse1')
  - [Mouse2](#F-gdio-unity_api-KeyCode-Mouse2 'gdio.unity_api.KeyCode.Mouse2')
  - [Mouse3](#F-gdio-unity_api-KeyCode-Mouse3 'gdio.unity_api.KeyCode.Mouse3')
  - [Mouse4](#F-gdio-unity_api-KeyCode-Mouse4 'gdio.unity_api.KeyCode.Mouse4')
  - [Mouse5](#F-gdio-unity_api-KeyCode-Mouse5 'gdio.unity_api.KeyCode.Mouse5')
  - [Mouse6](#F-gdio-unity_api-KeyCode-Mouse6 'gdio.unity_api.KeyCode.Mouse6')
  - [N](#F-gdio-unity_api-KeyCode-N 'gdio.unity_api.KeyCode.N')
  - [None](#F-gdio-unity_api-KeyCode-None 'gdio.unity_api.KeyCode.None')
  - [Numlock](#F-gdio-unity_api-KeyCode-Numlock 'gdio.unity_api.KeyCode.Numlock')
  - [O](#F-gdio-unity_api-KeyCode-O 'gdio.unity_api.KeyCode.O')
  - [P](#F-gdio-unity_api-KeyCode-P 'gdio.unity_api.KeyCode.P')
  - [PageDown](#F-gdio-unity_api-KeyCode-PageDown 'gdio.unity_api.KeyCode.PageDown')
  - [PageUp](#F-gdio-unity_api-KeyCode-PageUp 'gdio.unity_api.KeyCode.PageUp')
  - [Pause](#F-gdio-unity_api-KeyCode-Pause 'gdio.unity_api.KeyCode.Pause')
  - [Period](#F-gdio-unity_api-KeyCode-Period 'gdio.unity_api.KeyCode.Period')
  - [Plus](#F-gdio-unity_api-KeyCode-Plus 'gdio.unity_api.KeyCode.Plus')
  - [Print](#F-gdio-unity_api-KeyCode-Print 'gdio.unity_api.KeyCode.Print')
  - [Q](#F-gdio-unity_api-KeyCode-Q 'gdio.unity_api.KeyCode.Q')
  - [Question](#F-gdio-unity_api-KeyCode-Question 'gdio.unity_api.KeyCode.Question')
  - [Quote](#F-gdio-unity_api-KeyCode-Quote 'gdio.unity_api.KeyCode.Quote')
  - [R](#F-gdio-unity_api-KeyCode-R 'gdio.unity_api.KeyCode.R')
  - [Return](#F-gdio-unity_api-KeyCode-Return 'gdio.unity_api.KeyCode.Return')
  - [RightAlt](#F-gdio-unity_api-KeyCode-RightAlt 'gdio.unity_api.KeyCode.RightAlt')
  - [RightApple](#F-gdio-unity_api-KeyCode-RightApple 'gdio.unity_api.KeyCode.RightApple')
  - [RightArrow](#F-gdio-unity_api-KeyCode-RightArrow 'gdio.unity_api.KeyCode.RightArrow')
  - [RightBracket](#F-gdio-unity_api-KeyCode-RightBracket 'gdio.unity_api.KeyCode.RightBracket')
  - [RightCommand](#F-gdio-unity_api-KeyCode-RightCommand 'gdio.unity_api.KeyCode.RightCommand')
  - [RightControl](#F-gdio-unity_api-KeyCode-RightControl 'gdio.unity_api.KeyCode.RightControl')
  - [RightParen](#F-gdio-unity_api-KeyCode-RightParen 'gdio.unity_api.KeyCode.RightParen')
  - [RightShift](#F-gdio-unity_api-KeyCode-RightShift 'gdio.unity_api.KeyCode.RightShift')
  - [RightWindows](#F-gdio-unity_api-KeyCode-RightWindows 'gdio.unity_api.KeyCode.RightWindows')
  - [S](#F-gdio-unity_api-KeyCode-S 'gdio.unity_api.KeyCode.S')
  - [ScrollLock](#F-gdio-unity_api-KeyCode-ScrollLock 'gdio.unity_api.KeyCode.ScrollLock')
  - [Semicolon](#F-gdio-unity_api-KeyCode-Semicolon 'gdio.unity_api.KeyCode.Semicolon')
  - [Slash](#F-gdio-unity_api-KeyCode-Slash 'gdio.unity_api.KeyCode.Slash')
  - [Space](#F-gdio-unity_api-KeyCode-Space 'gdio.unity_api.KeyCode.Space')
  - [SysReq](#F-gdio-unity_api-KeyCode-SysReq 'gdio.unity_api.KeyCode.SysReq')
  - [T](#F-gdio-unity_api-KeyCode-T 'gdio.unity_api.KeyCode.T')
  - [Tab](#F-gdio-unity_api-KeyCode-Tab 'gdio.unity_api.KeyCode.Tab')
  - [U](#F-gdio-unity_api-KeyCode-U 'gdio.unity_api.KeyCode.U')
  - [Underscore](#F-gdio-unity_api-KeyCode-Underscore 'gdio.unity_api.KeyCode.Underscore')
  - [UpArrow](#F-gdio-unity_api-KeyCode-UpArrow 'gdio.unity_api.KeyCode.UpArrow')
  - [V](#F-gdio-unity_api-KeyCode-V 'gdio.unity_api.KeyCode.V')
  - [W](#F-gdio-unity_api-KeyCode-W 'gdio.unity_api.KeyCode.W')
  - [X](#F-gdio-unity_api-KeyCode-X 'gdio.unity_api.KeyCode.X')
  - [Y](#F-gdio-unity_api-KeyCode-Y 'gdio.unity_api.KeyCode.Y')
  - [Z](#F-gdio-unity_api-KeyCode-Z 'gdio.unity_api.KeyCode.Z')
- [ScreenCapture](#T-gdio-unity_api-utilities-ScreenCapture 'gdio.unity_api.utilities.ScreenCapture')
  - [CaptureScreen()](#M-gdio-unity_api-utilities-ScreenCapture-CaptureScreen 'gdio.unity_api.utilities.ScreenCapture.CaptureScreen')
  - [CaptureScreenToFile(filename,format)](#M-gdio-unity_api-utilities-ScreenCapture-CaptureScreenToFile-System-String,System-Drawing-Imaging-ImageFormat- 'gdio.unity_api.utilities.ScreenCapture.CaptureScreenToFile(System.String,System.Drawing.Imaging.ImageFormat)')
  - [CaptureWindow(handle)](#M-gdio-unity_api-utilities-ScreenCapture-CaptureWindow-System-IntPtr- 'gdio.unity_api.utilities.ScreenCapture.CaptureWindow(System.IntPtr)')
  - [CaptureWindowToFile(handle,filename,format)](#M-gdio-unity_api-utilities-ScreenCapture-CaptureWindowToFile-System-IntPtr,System-String,System-Drawing-Imaging-ImageFormat- 'gdio.unity_api.utilities.ScreenCapture.CaptureWindowToFile(System.IntPtr,System.String,System.Drawing.Imaging.ImageFormat)')
- [User32](#T-gdio-unity_api-utilities-ScreenCapture-User32 'gdio.unity_api.utilities.ScreenCapture.User32')
<a name='T-gdio-unity_api-utilities-ScreenCapture-GDI32'></a>

## GDI32 `type`

##### Namespace

gdio.unity_api.utilities.ScreenCapture

##### Summary

Helper class containing Gdi32 API functions

<a name='T-gdio-unity_api-v2-GameConnectionDetails'></a>
## GameConnectionDetails `type`

##### Namespace

gdio.unity_api.v2

##### Summary

This class provides information about the currently connected game.

<a name='F-gdio-unity_api-v2-GameConnectionDetails-Addr'></a>
### Addr `constants`

##### Summary

The [IPAddress](https://docs.microsoft.com/en-us/dotnet/api/System.Net.IPAddress 'System.Net.IPAddress') of the connected game./>

<a name='F-gdio-unity_api-v2-GameConnectionDetails-GamePath'></a>
### GamePath `constants`

##### Summary

The Application.DataPath of the connected game.

<a name='F-gdio-unity_api-v2-GameConnectionDetails-IsEditor'></a>
### IsEditor `constants`

##### Summary

Boolean value if the game is running in an Unity editor instance.

<a name='F-gdio-unity_api-v2-GameConnectionDetails-IsStandalone'></a>
### IsStandalone `constants`

##### Summary

Boolean value if the game is running as a Standalone instance.

<a name='F-gdio-unity_api-v2-GameConnectionDetails-Platform'></a>
### Platform `constants`

##### Summary

The Application.Platform of the connected game.

<a name='F-gdio-unity_api-v2-GameConnectionDetails-Port'></a>
### Port `constants`

##### Summary

The port number of the connected game.

<a name='T-gdio-unity_api-v2-HookingObject'></a>
## HookingObject `type`

##### Namespace

gdio.unity_api.v2

##### Summary

Enumeration of input types that can be hooked.  Currently TOUCHINPUT is bundled with MOUSE and GAMEPAD is not supported.

<a name='F-gdio-unity_api-v2-HookingObject-ALL'></a>
### ALL `constants`

##### Summary

All inputs

<a name='F-gdio-unity_api-v2-HookingObject-GAMEPAD'></a>
### GAMEPAD `constants`

##### Summary

Gamepad input, CURRENTLY NOT SUPPORTED

<a name='F-gdio-unity_api-v2-HookingObject-KEYBOARD'></a>
### KEYBOARD `constants`

##### Summary

Keyboard input

<a name='F-gdio-unity_api-v2-HookingObject-MOUSE'></a>
### MOUSE `constants`

##### Summary

Mouse input

<a name='F-gdio-unity_api-v2-HookingObject-TOUCHINPUT'></a>
### TOUCHINPUT `constants`

##### Summary

Touch input, enum value is currently not used.  Enabled/Disabled via [MOUSE](#F-gdio-unity_api-v2-HookingObject-MOUSE 'gdio.unity_api.v2.HookingObject.MOUSE') enumeration.

<a name='T-gdio-unity_api-KeyCode'></a>
## KeyCode `type`

##### Namespace

gdio.unity_api

##### Summary

Key codes returned by Event keyCode. These map directly to a physical key on the keyboard.

<a name='F-gdio-unity_api-KeyCode-A'></a>
### A `constants`

##### Summary

a' key

<a name='F-gdio-unity_api-KeyCode-Alpha0'></a>
### Alpha0 `constants`

##### Summary

The '0' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha1'></a>
### Alpha1 `constants`

##### Summary

The '1' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha2'></a>
### Alpha2 `constants`

##### Summary

The '2' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha3'></a>
### Alpha3 `constants`

##### Summary

The '3' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha4'></a>
### Alpha4 `constants`

##### Summary

The '4' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha5'></a>
### Alpha5 `constants`

##### Summary

The '5' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha6'></a>
### Alpha6 `constants`

##### Summary

The '6' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha7'></a>
### Alpha7 `constants`

##### Summary

The '7' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha8'></a>
### Alpha8 `constants`

##### Summary

The '8' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha9'></a>
### Alpha9 `constants`

##### Summary

The '9' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-AltGr'></a>
### AltGr `constants`

##### Summary

Alt Gr key

<a name='F-gdio-unity_api-KeyCode-Ampersand'></a>
### Ampersand `constants`

##### Summary

Ampersand key &

<a name='F-gdio-unity_api-KeyCode-Asterisk'></a>
### Asterisk `constants`

##### Summary

Asterisk key '*'

<a name='F-gdio-unity_api-KeyCode-At'></a>
### At `constants`

##### Summary

At key '@'

<a name='F-gdio-unity_api-KeyCode-B'></a>
### B `constants`

##### Summary

b' key

<a name='F-gdio-unity_api-KeyCode-BackQuote'></a>
### BackQuote `constants`

##### Summary

Back quote key '\`'

<a name='F-gdio-unity_api-KeyCode-Backslash'></a>
### Backslash `constants`

##### Summary

Backslash key '\'

<a name='F-gdio-unity_api-KeyCode-Backspace'></a>
### Backspace `constants`

##### Summary

The backspace key

<a name='F-gdio-unity_api-KeyCode-Break'></a>
### Break `constants`

##### Summary

Break key

<a name='F-gdio-unity_api-KeyCode-C'></a>
### C `constants`

##### Summary

c' key

<a name='F-gdio-unity_api-KeyCode-CapsLock'></a>
### CapsLock `constants`

##### Summary

Capslock key

<a name='F-gdio-unity_api-KeyCode-Caret'></a>
### Caret `constants`

##### Summary

Caret key '^'

<a name='F-gdio-unity_api-KeyCode-Clear'></a>
### Clear `constants`

##### Summary

The Clear key

<a name='F-gdio-unity_api-KeyCode-Colon'></a>
### Colon `constants`

##### Summary

Colon ':' key

<a name='F-gdio-unity_api-KeyCode-Comma'></a>
### Comma `constants`

##### Summary

Comma ',' key

<a name='F-gdio-unity_api-KeyCode-D'></a>
### D `constants`

##### Summary

d' key

<a name='F-gdio-unity_api-KeyCode-Delete'></a>
### Delete `constants`

##### Summary

The forward delete key

<a name='F-gdio-unity_api-KeyCode-Dollar'></a>
### Dollar `constants`

##### Summary

Dollar sign key $

<a name='F-gdio-unity_api-KeyCode-DoubleQuote'></a>
### DoubleQuote `constants`

##### Summary

Double quote key "

<a name='F-gdio-unity_api-KeyCode-DownArrow'></a>
### DownArrow `constants`

##### Summary

Down arrow key

<a name='F-gdio-unity_api-KeyCode-E'></a>
### E `constants`

##### Summary

e' key

<a name='F-gdio-unity_api-KeyCode-End'></a>
### End `constants`

##### Summary

End key

<a name='F-gdio-unity_api-KeyCode-Equals'></a>
### Equals `constants`

##### Summary

Equals '=' key

<a name='F-gdio-unity_api-KeyCode-Escape'></a>
### Escape `constants`

##### Summary

Escape key

<a name='F-gdio-unity_api-KeyCode-Exclaim'></a>
### Exclaim `constants`

##### Summary

Exclamation mark key !

<a name='F-gdio-unity_api-KeyCode-F'></a>
### F `constants`

##### Summary

f' key

<a name='F-gdio-unity_api-KeyCode-F1'></a>
### F1 `constants`

##### Summary

F1 function key

<a name='F-gdio-unity_api-KeyCode-F10'></a>
### F10 `constants`

##### Summary

F10 function key

<a name='F-gdio-unity_api-KeyCode-F11'></a>
### F11 `constants`

##### Summary

F11 function key

<a name='F-gdio-unity_api-KeyCode-F12'></a>
### F12 `constants`

##### Summary

F12 function key

<a name='F-gdio-unity_api-KeyCode-F13'></a>
### F13 `constants`

##### Summary

F13 function key

<a name='F-gdio-unity_api-KeyCode-F14'></a>
### F14 `constants`

##### Summary

F14 function key

<a name='F-gdio-unity_api-KeyCode-F15'></a>
### F15 `constants`

##### Summary

F15 function key

<a name='F-gdio-unity_api-KeyCode-F2'></a>
### F2 `constants`

##### Summary

F2 function key

<a name='F-gdio-unity_api-KeyCode-F3'></a>
### F3 `constants`

##### Summary

F3 function key

<a name='F-gdio-unity_api-KeyCode-F4'></a>
### F4 `constants`

##### Summary

F4 function key

<a name='F-gdio-unity_api-KeyCode-F5'></a>
### F5 `constants`

##### Summary

F5 function key

<a name='F-gdio-unity_api-KeyCode-F6'></a>
### F6 `constants`

##### Summary

F6 function key

<a name='F-gdio-unity_api-KeyCode-F7'></a>
### F7 `constants`

##### Summary

F7 function key

<a name='F-gdio-unity_api-KeyCode-F8'></a>
### F8 `constants`

##### Summary

F8 function key

<a name='F-gdio-unity_api-KeyCode-F9'></a>
### F9 `constants`

##### Summary

F9 function key

<a name='F-gdio-unity_api-KeyCode-G'></a>
### G `constants`

##### Summary

g' key

<a name='F-gdio-unity_api-KeyCode-Greater'></a>
### Greater `constants`

##### Summary

Greater than '>' key

<a name='F-gdio-unity_api-KeyCode-H'></a>
### H `constants`

##### Summary

h' key

<a name='F-gdio-unity_api-KeyCode-Hash'></a>
### Hash `constants`

##### Summary

Hash key #

<a name='F-gdio-unity_api-KeyCode-Help'></a>
### Help `constants`

##### Summary

Help key

<a name='F-gdio-unity_api-KeyCode-Home'></a>
### Home `constants`

##### Summary

Home key

<a name='F-gdio-unity_api-KeyCode-I'></a>
### I `constants`

##### Summary

i' key

<a name='F-gdio-unity_api-KeyCode-Insert'></a>
### Insert `constants`

##### Summary

Insert key key

<a name='F-gdio-unity_api-KeyCode-J'></a>
### J `constants`

##### Summary

j' key

<a name='F-gdio-unity_api-KeyCode-Joystick1Button0'></a>
### Joystick1Button0 `constants`

##### Summary

Button 0 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button1'></a>
### Joystick1Button1 `constants`

##### Summary

Button 1 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button10'></a>
### Joystick1Button10 `constants`

##### Summary

Button 10 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button11'></a>
### Joystick1Button11 `constants`

##### Summary

Button 11 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button12'></a>
### Joystick1Button12 `constants`

##### Summary

Button 12 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button13'></a>
### Joystick1Button13 `constants`

##### Summary

Button 13 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button14'></a>
### Joystick1Button14 `constants`

##### Summary

Button 14 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button15'></a>
### Joystick1Button15 `constants`

##### Summary

Button 15 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button16'></a>
### Joystick1Button16 `constants`

##### Summary

Button 16 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button17'></a>
### Joystick1Button17 `constants`

##### Summary

Button 17 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button18'></a>
### Joystick1Button18 `constants`

##### Summary

Button 18 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button19'></a>
### Joystick1Button19 `constants`

##### Summary

Button 19 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button2'></a>
### Joystick1Button2 `constants`

##### Summary

Button 2 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button3'></a>
### Joystick1Button3 `constants`

##### Summary

Button 3 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button4'></a>
### Joystick1Button4 `constants`

##### Summary

Button 4 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button5'></a>
### Joystick1Button5 `constants`

##### Summary

Button 5 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button6'></a>
### Joystick1Button6 `constants`

##### Summary

Button 6 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button7'></a>
### Joystick1Button7 `constants`

##### Summary

Button 7 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button8'></a>
### Joystick1Button8 `constants`

##### Summary

Button 8 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button9'></a>
### Joystick1Button9 `constants`

##### Summary

Button 9 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button0'></a>
### Joystick2Button0 `constants`

##### Summary

Button 0 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button1'></a>
### Joystick2Button1 `constants`

##### Summary

Button 1 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button10'></a>
### Joystick2Button10 `constants`

##### Summary

Button 10 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button11'></a>
### Joystick2Button11 `constants`

##### Summary

Button 11 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button12'></a>
### Joystick2Button12 `constants`

##### Summary

Button 12 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button13'></a>
### Joystick2Button13 `constants`

##### Summary

Button 13 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button14'></a>
### Joystick2Button14 `constants`

##### Summary

Button 14 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button15'></a>
### Joystick2Button15 `constants`

##### Summary

Button 15 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button16'></a>
### Joystick2Button16 `constants`

##### Summary

Button 16 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button17'></a>
### Joystick2Button17 `constants`

##### Summary

Button 17 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button18'></a>
### Joystick2Button18 `constants`

##### Summary

Button 18 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button19'></a>
### Joystick2Button19 `constants`

##### Summary

Button 19 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button2'></a>
### Joystick2Button2 `constants`

##### Summary

Button 2 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button3'></a>
### Joystick2Button3 `constants`

##### Summary

Button 3 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button4'></a>
### Joystick2Button4 `constants`

##### Summary

Button 4 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button5'></a>
### Joystick2Button5 `constants`

##### Summary

Button 5 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button6'></a>
### Joystick2Button6 `constants`

##### Summary

Button 6 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button7'></a>
### Joystick2Button7 `constants`

##### Summary

Button 7 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button8'></a>
### Joystick2Button8 `constants`

##### Summary

Button 8 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button9'></a>
### Joystick2Button9 `constants`

##### Summary

Button 9 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button0'></a>
### Joystick3Button0 `constants`

##### Summary

Button 0 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button1'></a>
### Joystick3Button1 `constants`

##### Summary

Button 1 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button10'></a>
### Joystick3Button10 `constants`

##### Summary

Button 10 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button11'></a>
### Joystick3Button11 `constants`

##### Summary

Button 11 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button12'></a>
### Joystick3Button12 `constants`

##### Summary

Button 12 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button13'></a>
### Joystick3Button13 `constants`

##### Summary

Button 13 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button14'></a>
### Joystick3Button14 `constants`

##### Summary

Button 14 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button15'></a>
### Joystick3Button15 `constants`

##### Summary

Button 15 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button16'></a>
### Joystick3Button16 `constants`

##### Summary

Button 16 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button17'></a>
### Joystick3Button17 `constants`

##### Summary

Button 17 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button18'></a>
### Joystick3Button18 `constants`

##### Summary

Button 18 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button19'></a>
### Joystick3Button19 `constants`

##### Summary

Button 19 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button2'></a>
### Joystick3Button2 `constants`

##### Summary

Button 2 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button3'></a>
### Joystick3Button3 `constants`

##### Summary

Button 3 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button4'></a>
### Joystick3Button4 `constants`

##### Summary

Button 4 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button5'></a>
### Joystick3Button5 `constants`

##### Summary

Button 5 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button6'></a>
### Joystick3Button6 `constants`

##### Summary

Button 6 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button7'></a>
### Joystick3Button7 `constants`

##### Summary

Button 7 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button8'></a>
### Joystick3Button8 `constants`

##### Summary

Button 8 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button9'></a>
### Joystick3Button9 `constants`

##### Summary

Button 9 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button0'></a>
### Joystick4Button0 `constants`

##### Summary

Button 0 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button1'></a>
### Joystick4Button1 `constants`

##### Summary

Button 1 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button10'></a>
### Joystick4Button10 `constants`

##### Summary

Button 10 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button11'></a>
### Joystick4Button11 `constants`

##### Summary

Button 11 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button12'></a>
### Joystick4Button12 `constants`

##### Summary

Button 12 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button13'></a>
### Joystick4Button13 `constants`

##### Summary

Button 13 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button14'></a>
### Joystick4Button14 `constants`

##### Summary

Button 14 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button15'></a>
### Joystick4Button15 `constants`

##### Summary

Button 15 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button16'></a>
### Joystick4Button16 `constants`

##### Summary

Button 16 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button17'></a>
### Joystick4Button17 `constants`

##### Summary

Button 17 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button18'></a>
### Joystick4Button18 `constants`

##### Summary

Button 18 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button19'></a>
### Joystick4Button19 `constants`

##### Summary

Button 19 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button2'></a>
### Joystick4Button2 `constants`

##### Summary

Button 2 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button3'></a>
### Joystick4Button3 `constants`

##### Summary

Button 3 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button4'></a>
### Joystick4Button4 `constants`

##### Summary

Button 4 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button5'></a>
### Joystick4Button5 `constants`

##### Summary

Button 5 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button6'></a>
### Joystick4Button6 `constants`

##### Summary

Button 6 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button7'></a>
### Joystick4Button7 `constants`

##### Summary

Button 7 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button8'></a>
### Joystick4Button8 `constants`

##### Summary

Button 8 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button9'></a>
### Joystick4Button9 `constants`

##### Summary

Button 9 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button0'></a>
### Joystick5Button0 `constants`

##### Summary

Button 0 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button1'></a>
### Joystick5Button1 `constants`

##### Summary

Button 1 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button10'></a>
### Joystick5Button10 `constants`

##### Summary

Button 10 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button11'></a>
### Joystick5Button11 `constants`

##### Summary

Button 11 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button12'></a>
### Joystick5Button12 `constants`

##### Summary

Button 12 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button13'></a>
### Joystick5Button13 `constants`

##### Summary

Button 13 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button14'></a>
### Joystick5Button14 `constants`

##### Summary

Button 14 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button15'></a>
### Joystick5Button15 `constants`

##### Summary

Button 15 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button16'></a>
### Joystick5Button16 `constants`

##### Summary

Button 16 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button17'></a>
### Joystick5Button17 `constants`

##### Summary

Button 17 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button18'></a>
### Joystick5Button18 `constants`

##### Summary

Button 18 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button19'></a>
### Joystick5Button19 `constants`

##### Summary

Button 19 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button2'></a>
### Joystick5Button2 `constants`

##### Summary

Button 2 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button3'></a>
### Joystick5Button3 `constants`

##### Summary

Button 3 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button4'></a>
### Joystick5Button4 `constants`

##### Summary

Button 4 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button5'></a>
### Joystick5Button5 `constants`

##### Summary

Button 5 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button6'></a>
### Joystick5Button6 `constants`

##### Summary

Button 6 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button7'></a>
### Joystick5Button7 `constants`

##### Summary

Button 7 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button8'></a>
### Joystick5Button8 `constants`

##### Summary

Button 8 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button9'></a>
### Joystick5Button9 `constants`

##### Summary

Button 9 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button0'></a>
### Joystick6Button0 `constants`

##### Summary

Button 0 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button1'></a>
### Joystick6Button1 `constants`

##### Summary

Button 1 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button10'></a>
### Joystick6Button10 `constants`

##### Summary

Button 10 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button11'></a>
### Joystick6Button11 `constants`

##### Summary

Button 11 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button12'></a>
### Joystick6Button12 `constants`

##### Summary

Button 12 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button13'></a>
### Joystick6Button13 `constants`

##### Summary

Button 13 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button14'></a>
### Joystick6Button14 `constants`

##### Summary

Button 14 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button15'></a>
### Joystick6Button15 `constants`

##### Summary

Button 15 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button16'></a>
### Joystick6Button16 `constants`

##### Summary

Button 16 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button17'></a>
### Joystick6Button17 `constants`

##### Summary

Button 17 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button18'></a>
### Joystick6Button18 `constants`

##### Summary

Button 18 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button19'></a>
### Joystick6Button19 `constants`

##### Summary

Button 19 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button2'></a>
### Joystick6Button2 `constants`

##### Summary

Button 2 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button3'></a>
### Joystick6Button3 `constants`

##### Summary

Button 3 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button4'></a>
### Joystick6Button4 `constants`

##### Summary

Button 4 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button5'></a>
### Joystick6Button5 `constants`

##### Summary

Button 5 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button6'></a>
### Joystick6Button6 `constants`

##### Summary

Button 6 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button7'></a>
### Joystick6Button7 `constants`

##### Summary

Button 7 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button8'></a>
### Joystick6Button8 `constants`

##### Summary

Button 8 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button9'></a>
### Joystick6Button9 `constants`

##### Summary

Button 9 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button0'></a>
### Joystick7Button0 `constants`

##### Summary

Button 0 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button1'></a>
### Joystick7Button1 `constants`

##### Summary

Button 1 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button10'></a>
### Joystick7Button10 `constants`

##### Summary

Button 10 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button11'></a>
### Joystick7Button11 `constants`

##### Summary

Button 11 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button12'></a>
### Joystick7Button12 `constants`

##### Summary

Button 12 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button13'></a>
### Joystick7Button13 `constants`

##### Summary

Button 13 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button14'></a>
### Joystick7Button14 `constants`

##### Summary

Button 14 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button15'></a>
### Joystick7Button15 `constants`

##### Summary

Button 15 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button16'></a>
### Joystick7Button16 `constants`

##### Summary

Button 16 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button17'></a>
### Joystick7Button17 `constants`

##### Summary

Button 17 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button18'></a>
### Joystick7Button18 `constants`

##### Summary

Button 18 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button19'></a>
### Joystick7Button19 `constants`

##### Summary

Button 19 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button2'></a>
### Joystick7Button2 `constants`

##### Summary

Button 2 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button3'></a>
### Joystick7Button3 `constants`

##### Summary

Button 3 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button4'></a>
### Joystick7Button4 `constants`

##### Summary

Button 4 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button5'></a>
### Joystick7Button5 `constants`

##### Summary

Button 5 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button6'></a>
### Joystick7Button6 `constants`

##### Summary

Button 6 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button7'></a>
### Joystick7Button7 `constants`

##### Summary

Button 7 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button8'></a>
### Joystick7Button8 `constants`

##### Summary

Button 8 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button9'></a>
### Joystick7Button9 `constants`

##### Summary

Button 9 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button0'></a>
### Joystick8Button0 `constants`

##### Summary

Button 0 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button1'></a>
### Joystick8Button1 `constants`

##### Summary

Button 1 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button10'></a>
### Joystick8Button10 `constants`

##### Summary

Button 10 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button11'></a>
### Joystick8Button11 `constants`

##### Summary

Button 11 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button12'></a>
### Joystick8Button12 `constants`

##### Summary

Button 12 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button13'></a>
### Joystick8Button13 `constants`

##### Summary

Button 13 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button14'></a>
### Joystick8Button14 `constants`

##### Summary

Button 14 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button15'></a>
### Joystick8Button15 `constants`

##### Summary

Button 15 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button16'></a>
### Joystick8Button16 `constants`

##### Summary

Button 16 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button17'></a>
### Joystick8Button17 `constants`

##### Summary

Button 17 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button18'></a>
### Joystick8Button18 `constants`

##### Summary

Button 18 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button19'></a>
### Joystick8Button19 `constants`

##### Summary

Button 19 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button2'></a>
### Joystick8Button2 `constants`

##### Summary

Button 2 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button3'></a>
### Joystick8Button3 `constants`

##### Summary

Button 3 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button4'></a>
### Joystick8Button4 `constants`

##### Summary

Button 4 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button5'></a>
### Joystick8Button5 `constants`

##### Summary

Button 5 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button6'></a>
### Joystick8Button6 `constants`

##### Summary

Button 6 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button7'></a>
### Joystick8Button7 `constants`

##### Summary

Button 7 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button8'></a>
### Joystick8Button8 `constants`

##### Summary

Button 8 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button9'></a>
### Joystick8Button9 `constants`

##### Summary

Button 9 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton0'></a>
### JoystickButton0 `constants`

##### Summary

Button 0 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton1'></a>
### JoystickButton1 `constants`

##### Summary

Button 1 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton10'></a>
### JoystickButton10 `constants`

##### Summary

Button 10 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton11'></a>
### JoystickButton11 `constants`

##### Summary

Button 11 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton12'></a>
### JoystickButton12 `constants`

##### Summary

Button 12 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton13'></a>
### JoystickButton13 `constants`

##### Summary

Button 13 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton14'></a>
### JoystickButton14 `constants`

##### Summary

Button 14 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton15'></a>
### JoystickButton15 `constants`

##### Summary

Button 15 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton16'></a>
### JoystickButton16 `constants`

##### Summary

Button 16 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton17'></a>
### JoystickButton17 `constants`

##### Summary

Button 17 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton18'></a>
### JoystickButton18 `constants`

##### Summary

Button 18 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton19'></a>
### JoystickButton19 `constants`

##### Summary

Button 19 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton2'></a>
### JoystickButton2 `constants`

##### Summary

Button 2 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton3'></a>
### JoystickButton3 `constants`

##### Summary

Button 3 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton4'></a>
### JoystickButton4 `constants`

##### Summary

Button 4 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton5'></a>
### JoystickButton5 `constants`

##### Summary

Button 5 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton6'></a>
### JoystickButton6 `constants`

##### Summary

Button 6 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton7'></a>
### JoystickButton7 `constants`

##### Summary

Button 7 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton8'></a>
### JoystickButton8 `constants`

##### Summary

Button 8 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton9'></a>
### JoystickButton9 `constants`

##### Summary

Button 9 on any joystick

<a name='F-gdio-unity_api-KeyCode-K'></a>
### K `constants`

##### Summary

k' key

<a name='F-gdio-unity_api-KeyCode-Keypad0'></a>
### Keypad0 `constants`

##### Summary

Numeric keypad 0

<a name='F-gdio-unity_api-KeyCode-Keypad1'></a>
### Keypad1 `constants`

##### Summary

Numeric keypad 1

<a name='F-gdio-unity_api-KeyCode-Keypad2'></a>
### Keypad2 `constants`

##### Summary

Numeric keypad 2

<a name='F-gdio-unity_api-KeyCode-Keypad3'></a>
### Keypad3 `constants`

##### Summary

Numeric keypad 3

<a name='F-gdio-unity_api-KeyCode-Keypad4'></a>
### Keypad4 `constants`

##### Summary

Numeric keypad 4

<a name='F-gdio-unity_api-KeyCode-Keypad5'></a>
### Keypad5 `constants`

##### Summary

Numeric keypad 5

<a name='F-gdio-unity_api-KeyCode-Keypad6'></a>
### Keypad6 `constants`

##### Summary

Numeric keypad 6

<a name='F-gdio-unity_api-KeyCode-Keypad7'></a>
### Keypad7 `constants`

##### Summary

Numeric keypad 7

<a name='F-gdio-unity_api-KeyCode-Keypad8'></a>
### Keypad8 `constants`

##### Summary

Numeric keypad 8

<a name='F-gdio-unity_api-KeyCode-Keypad9'></a>
### Keypad9 `constants`

##### Summary

Numeric keypad 9

<a name='F-gdio-unity_api-KeyCode-KeypadDivide'></a>
### KeypadDivide `constants`

##### Summary

Numeric keypad '/'

<a name='F-gdio-unity_api-KeyCode-KeypadEnter'></a>
### KeypadEnter `constants`

##### Summary

Numeric keypad enter

<a name='F-gdio-unity_api-KeyCode-KeypadEquals'></a>
### KeypadEquals `constants`

##### Summary

Numeric keypad '='

<a name='F-gdio-unity_api-KeyCode-KeypadMinus'></a>
### KeypadMinus `constants`

##### Summary

Numeric keypad '-'

<a name='F-gdio-unity_api-KeyCode-KeypadMultiply'></a>
### KeypadMultiply `constants`

##### Summary

Numeric keypad '*'

<a name='F-gdio-unity_api-KeyCode-KeypadPeriod'></a>
### KeypadPeriod `constants`

##### Summary

Numeric keypad '

<a name='F-gdio-unity_api-KeyCode-KeypadPlus'></a>
### KeypadPlus `constants`

##### Summary

Numeric keypad '+'

<a name='F-gdio-unity_api-KeyCode-L'></a>
### L `constants`

##### Summary

l' key

<a name='F-gdio-unity_api-KeyCode-LeftAlt'></a>
### LeftAlt `constants`

##### Summary

Left Alt key

<a name='F-gdio-unity_api-KeyCode-LeftApple'></a>
### LeftApple `constants`

##### Summary

Left Command key

<a name='F-gdio-unity_api-KeyCode-LeftArrow'></a>
### LeftArrow `constants`

##### Summary

Left arrow key

<a name='F-gdio-unity_api-KeyCode-LeftBracket'></a>
### LeftBracket `constants`

##### Summary

Left square bracket key '['

<a name='F-gdio-unity_api-KeyCode-LeftCommand'></a>
### LeftCommand `constants`

##### Summary

Left Command key

<a name='F-gdio-unity_api-KeyCode-LeftControl'></a>
### LeftControl `constants`

##### Summary

Left Control key

<a name='F-gdio-unity_api-KeyCode-LeftParen'></a>
### LeftParen `constants`

##### Summary

Left Parenthesis key '('

<a name='F-gdio-unity_api-KeyCode-LeftShift'></a>
### LeftShift `constants`

##### Summary

Left shift key

<a name='F-gdio-unity_api-KeyCode-LeftWindows'></a>
### LeftWindows `constants`

##### Summary

Left Windows key

<a name='F-gdio-unity_api-KeyCode-Less'></a>
### Less `constants`

##### Summary

Less than '<' key

<a name='F-gdio-unity_api-KeyCode-M'></a>
### M `constants`

##### Summary

m' key

<a name='F-gdio-unity_api-KeyCode-Menu'></a>
### Menu `constants`

##### Summary

Menu key

<a name='F-gdio-unity_api-KeyCode-Minus'></a>
### Minus `constants`

##### Summary

Minus '-' key

<a name='F-gdio-unity_api-KeyCode-Mouse0'></a>
### Mouse0 `constants`

##### Summary

The Left (or primary) mouse button

<a name='F-gdio-unity_api-KeyCode-Mouse1'></a>
### Mouse1 `constants`

##### Summary

Right mouse button (or secondary mouse button)

<a name='F-gdio-unity_api-KeyCode-Mouse2'></a>
### Mouse2 `constants`

##### Summary

Middle mouse button (or third button)

<a name='F-gdio-unity_api-KeyCode-Mouse3'></a>
### Mouse3 `constants`

##### Summary

Additional (fourth) mouse button

<a name='F-gdio-unity_api-KeyCode-Mouse4'></a>
### Mouse4 `constants`

##### Summary

Additional (fifth) mouse button

<a name='F-gdio-unity_api-KeyCode-Mouse5'></a>
### Mouse5 `constants`

##### Summary

Additional (or sixth) mouse button

<a name='F-gdio-unity_api-KeyCode-Mouse6'></a>
### Mouse6 `constants`

##### Summary

Additional (or seventh) mouse button

<a name='F-gdio-unity_api-KeyCode-N'></a>
### N `constants`

##### Summary

n' key

<a name='F-gdio-unity_api-KeyCode-None'></a>
### None `constants`

##### Summary

Not assigned (never returned as the result of a keystroke)

<a name='F-gdio-unity_api-KeyCode-Numlock'></a>
### Numlock `constants`

##### Summary

Numlock key

<a name='F-gdio-unity_api-KeyCode-O'></a>
### O `constants`

##### Summary

o' key

<a name='F-gdio-unity_api-KeyCode-P'></a>
### P `constants`

##### Summary

p' key

<a name='F-gdio-unity_api-KeyCode-PageDown'></a>
### PageDown `constants`

##### Summary

Page down

<a name='F-gdio-unity_api-KeyCode-PageUp'></a>
### PageUp `constants`

##### Summary

Page up

<a name='F-gdio-unity_api-KeyCode-Pause'></a>
### Pause `constants`

##### Summary

Pause on PC machines

<a name='F-gdio-unity_api-KeyCode-Period'></a>
### Period `constants`

##### Summary

Period '

<a name='F-gdio-unity_api-KeyCode-Plus'></a>
### Plus `constants`

##### Summary

Plus key '+'

<a name='F-gdio-unity_api-KeyCode-Print'></a>
### Print `constants`

##### Summary

Print key

<a name='F-gdio-unity_api-KeyCode-Q'></a>
### Q `constants`

##### Summary

q' key

<a name='F-gdio-unity_api-KeyCode-Question'></a>
### Question `constants`

##### Summary

Question mark '?' key

<a name='F-gdio-unity_api-KeyCode-Quote'></a>
### Quote `constants`

##### Summary

Quote key '

<a name='F-gdio-unity_api-KeyCode-R'></a>
### R `constants`

##### Summary

r' key

<a name='F-gdio-unity_api-KeyCode-Return'></a>
### Return `constants`

##### Summary

Return key

<a name='F-gdio-unity_api-KeyCode-RightAlt'></a>
### RightAlt `constants`

##### Summary

Right Alt key

<a name='F-gdio-unity_api-KeyCode-RightApple'></a>
### RightApple `constants`

##### Summary

Right Command key

<a name='F-gdio-unity_api-KeyCode-RightArrow'></a>
### RightArrow `constants`

##### Summary

Right arrow key

<a name='F-gdio-unity_api-KeyCode-RightBracket'></a>
### RightBracket `constants`

##### Summary

Right square bracket key ']'

<a name='F-gdio-unity_api-KeyCode-RightCommand'></a>
### RightCommand `constants`

##### Summary

Right Command key

<a name='F-gdio-unity_api-KeyCode-RightControl'></a>
### RightControl `constants`

##### Summary

Right Control key

<a name='F-gdio-unity_api-KeyCode-RightParen'></a>
### RightParen `constants`

##### Summary

Right Parenthesis key ')'

<a name='F-gdio-unity_api-KeyCode-RightShift'></a>
### RightShift `constants`

##### Summary

Right shift key

<a name='F-gdio-unity_api-KeyCode-RightWindows'></a>
### RightWindows `constants`

##### Summary

Right Windows key

<a name='F-gdio-unity_api-KeyCode-S'></a>
### S `constants`

##### Summary

s' key

<a name='F-gdio-unity_api-KeyCode-ScrollLock'></a>
### ScrollLock `constants`

##### Summary

Scroll lock key

<a name='F-gdio-unity_api-KeyCode-Semicolon'></a>
### Semicolon `constants`

##### Summary

Semicolon ';' key

<a name='F-gdio-unity_api-KeyCode-Slash'></a>
### Slash `constants`

##### Summary

Slash '/' key

<a name='F-gdio-unity_api-KeyCode-Space'></a>
### Space `constants`

##### Summary

Space key

<a name='F-gdio-unity_api-KeyCode-SysReq'></a>
### SysReq `constants`

##### Summary

Sys Req key

<a name='F-gdio-unity_api-KeyCode-T'></a>
### T `constants`

##### Summary

t' key

<a name='F-gdio-unity_api-KeyCode-Tab'></a>
### Tab `constants`

##### Summary

The tab key

<a name='F-gdio-unity_api-KeyCode-U'></a>
### U `constants`

##### Summary

u' key

<a name='F-gdio-unity_api-KeyCode-Underscore'></a>
### Underscore `constants`

##### Summary

Underscore '_' key

<a name='F-gdio-unity_api-KeyCode-UpArrow'></a>
### UpArrow `constants`

##### Summary

Up arrow key

<a name='F-gdio-unity_api-KeyCode-V'></a>
### V `constants`

##### Summary

v' key

<a name='F-gdio-unity_api-KeyCode-W'></a>
### W `constants`

##### Summary

w' key

<a name='F-gdio-unity_api-KeyCode-X'></a>
### X `constants`

##### Summary

x' key

<a name='F-gdio-unity_api-KeyCode-Y'></a>
### Y `constants`

##### Summary

y' key

<a name='F-gdio-unity_api-KeyCode-Z'></a>
### Z `constants`

##### Summary

z' key

