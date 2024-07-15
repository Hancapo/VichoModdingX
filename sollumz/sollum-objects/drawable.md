# ✈️ Drawable

## Specification

A [Drawable](drawable.md) is the top-most object of a YDR or one of the multiple children that a YDD can have.

## Parameters

| Parameter             | Meaning                                                             |
| --------------------- | ------------------------------------------------------------------- |
| `Lod Distance High`   | Render distance in units for the high lod model if there's any.     |
| `Lod Distance Medium` | Render distance in units for the medium lod model if there's any.   |
| `Lod Distance Low`    | Render distance in units for the low lod model if there's any.      |
| `Lod Distance Vlow`   | Render distance in units for the very low lod model if there's any. |

{% hint style="info" %}
For [drawables](drawable.md) that just have one LOD level (usually a high LOD) all 4 values are set to 9998, this setting can be tweaked to customize the render distance of the different LODs if there's more than one (the High one).
{% endhint %}

{% hint style="success" %}
Entity Definition tab it is used to set YMAP entity definitions.
{% endhint %}
