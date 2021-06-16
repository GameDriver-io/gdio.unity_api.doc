<a name='assembly'></a>
# gdio.common.objects

## Contents

- [CoordinateConversion](#T-gdio-common-objects-CoordinateConversion 'gdio.common.objects.CoordinateConversion')
  - [Local](#F-gdio-common-objects-CoordinateConversion-Local 'gdio.common.objects.CoordinateConversion.Local')
  - [None](#F-gdio-common-objects-CoordinateConversion-None 'gdio.common.objects.CoordinateConversion.None')
  - [ScreenToViewportPoint](#F-gdio-common-objects-CoordinateConversion-ScreenToViewportPoint 'gdio.common.objects.CoordinateConversion.ScreenToViewportPoint')
  - [ScreenToWorldPoint](#F-gdio-common-objects-CoordinateConversion-ScreenToWorldPoint 'gdio.common.objects.CoordinateConversion.ScreenToWorldPoint')
  - [ViewportToScreenPoint](#F-gdio-common-objects-CoordinateConversion-ViewportToScreenPoint 'gdio.common.objects.CoordinateConversion.ViewportToScreenPoint')
  - [ViewportToWorldPoint](#F-gdio-common-objects-CoordinateConversion-ViewportToWorldPoint 'gdio.common.objects.CoordinateConversion.ViewportToWorldPoint')
  - [WorldToScreenPoint](#F-gdio-common-objects-CoordinateConversion-WorldToScreenPoint 'gdio.common.objects.CoordinateConversion.WorldToScreenPoint')
  - [WorldToViewportPoint](#F-gdio-common-objects-CoordinateConversion-WorldToViewportPoint 'gdio.common.objects.CoordinateConversion.WorldToViewportPoint')
- [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons')
  - [LEFT](#F-gdio-common-objects-MouseButtons-LEFT 'gdio.common.objects.MouseButtons.LEFT')
  - [MIDDLE](#F-gdio-common-objects-MouseButtons-MIDDLE 'gdio.common.objects.MouseButtons.MIDDLE')
  - [RIGHT](#F-gdio-common-objects-MouseButtons-RIGHT 'gdio.common.objects.MouseButtons.RIGHT')
- [ObjectListFilter](#T-gdio-common-objects-ObjectListFilter 'gdio.common.objects.ObjectListFilter')
  - [ALL](#F-gdio-common-objects-ObjectListFilter-ALL 'gdio.common.objects.ObjectListFilter.ALL')
  - [TAGGED](#F-gdio-common-objects-ObjectListFilter-TAGGED 'gdio.common.objects.ObjectListFilter.TAGGED')
  - [UNTAGGED](#F-gdio-common-objects-ObjectListFilter-UNTAGGED 'gdio.common.objects.ObjectListFilter.UNTAGGED')

<a name='T-gdio-common-objects-CoordinateConversion'></a>
## CoordinateConversion `type`

##### Namespace

gdio.common.objects

<a name='F-gdio-common-objects-CoordinateConversion-Local'></a>
### Local `constants`

##### Summary

Local returns the gameObject.transform.localposition without any conversion

<a name='F-gdio-common-objects-CoordinateConversion-None'></a>
### None `constants`

##### Summary

None returns the gameObject.transform.position without any conversion

<a name='F-gdio-common-objects-CoordinateConversion-ScreenToViewportPoint'></a>
### ScreenToViewportPoint `constants`

##### Summary

ScreenToViewPortPoint returns the coordinates of the object in the viewport space of the specified Camera.  The default is Camera.main.

<a name='F-gdio-common-objects-CoordinateConversion-ScreenToWorldPoint'></a>
### ScreenToWorldPoint `constants`

##### Summary

ScreenToWorldPoint returns the coordinates of the object in the world space of the specified Camera.  The default is Camera.main.

<a name='F-gdio-common-objects-CoordinateConversion-ViewportToScreenPoint'></a>
### ViewportToScreenPoint `constants`

##### Summary

ScreenToViewPortPoint returns the coordinates of the object in the viewport space of the specified Camera.  The default is Camera.main.

<a name='F-gdio-common-objects-CoordinateConversion-ViewportToWorldPoint'></a>
### ViewportToWorldPoint `constants`

##### Summary

ScreenToWorldPoint returns the coordinates of the object in the world space of the specified Camera.  The default is Camera.main.

<a name='F-gdio-common-objects-CoordinateConversion-WorldToScreenPoint'></a>
### WorldToScreenPoint `constants`

##### Summary

WorldToScreenPoint returns the coordinates of the object transformed from World-To-Screen by the specified Camera.  The default is Camera.main.

<a name='F-gdio-common-objects-CoordinateConversion-WorldToViewportPoint'></a>
### WorldToViewportPoint `constants`

##### Summary

WorldToViewPortPoint returns the coordinates of the object in the screen space of the specified Camera.  The default is Camera.main.

<a name='T-gdio-common-objects-MouseButtons'></a>
## MouseButtons `type`

##### Namespace

gdio.common.objects

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
