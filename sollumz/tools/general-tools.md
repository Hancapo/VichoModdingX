# 🔧 General Tools

<table data-view="cards"><thead><tr><th align="center"></th><th align="center"></th><th align="center"></th></tr></thead><tbody><tr><td align="center">Import CodeWalker XML</td><td align="center"></td><td align="center">Quick shortcut to import CodeWalker XML files</td></tr><tr><td align="center">Export CodeWalker XML</td><td align="center"></td><td align="center">Quick shortcut to export CodeWalker XML files</td></tr></tbody></table>

***

## 💻 View

<table data-view="cards"><thead><tr><th align="center"></th><th align="center"></th></tr></thead><tbody><tr><td align="center">Hide Collisions</td><td align="center">Hides all Sollum collisions in the scene</td></tr><tr><td align="center">Hide Shattermaps</td><td align="center">Hides all vehicle shattermaps in the scene</td></tr></tbody></table>

***

### Level of Detail

<table data-view="cards"><thead><tr><th align="center"></th><th align="center"></th></tr></thead><tbody><tr><td align="center">Very High</td><td align="center">Set the viewing level to Very High for the selected Drawables/Fragments</td></tr><tr><td align="center">High</td><td align="center">Set the viewing level to High for the selected Drawables/Fragments</td></tr><tr><td align="center">Medium</td><td align="center">Set the viewing level to Medium for the selected Drawables/Fragments</td></tr><tr><td align="center">Low</td><td align="center">Set the viewing level to Low for the selected Drawables/Fragments</td></tr><tr><td align="center">Very Low</td><td align="center">Set the viewing level to Very Low for the selected Drawables/Fragments</td></tr><tr><td align="center">Hidden</td><td align="center">Hides all LOD levels for the selected Drawables/Fragments</td></tr></tbody></table>

## 🪥 Vertex Painter

Paints all vertex of the desired color in selected objects, it just works for [Drawable Model](../sollum-objects/drawable-model.md).

{% hint style="info" %}
The current vertex painter tools contain 6 palettes.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

## 🪣 Terrain Painter

{% hint style="info" %}
You must be in Vertex Paint mode to use it.
{% endhint %}

|                 |                                                                                                   |
| --------------- | ------------------------------------------------------------------------------------------------- |
| Paint Texture 1 | Sets brush blending mode to Mix and Brush Color to Black (RGB: 0,0,0)                             |
| Paint Texture 2 | Sets brush blending mode to Mix and Brush Color to Blue (RGB: 0,0,1)                              |
| Paint Texture 3 | Sets brush blending mode to Mix and Brush Color to Green (RGB: 0,1,0)                             |
| Paint Texture 4 | Sets brush blending mode to Mix and Brush Color to Cyan (RGB: 0,1,1)                              |
| Paint Alpha     | Sets brush blending mode to Add Alpha if Alpha value is above 0.0 or Erase Alpha if is below 0.0. |
| Alpha           | From -1.0 to 1.0, sets the Strength of the alpha brush.                                           |

{% hint style="info" %}
It creates a new brush for Vertex Paint called `TerrainBrush`.
{% endhint %}

{% hint style="warning" %}
Requires a secondary vertex color channel called `Color 1`
{% endhint %}

{% hint style="warning" %}
Requires a compatible terrain shader to work with, such as `terrain_cb_w_4lyr`
{% endhint %}

## 🐛 Debug

#### Fix Hierarchy

It will try to fix the hierarchy of the Sollumz objects in the scene, you must select the type in the `Hierarchy Type` drop-down control.

{% hint style="info" %}
Available types: Drawable, Drawable Dictionary and Bound Composite
{% endhint %}

#### Set Sollum Type

Changes the Sollum type of any selected object, even if this object had no Sollumz type before to the selected one.

{% hint style="info" %}
It supports **all** Sollum types available to the date.
{% endhint %}

#### Re-adjust Light Intensity

{% hint style="info" %}
It multiplies light intensity by a factor of 500 to make older projects compatible with the light intensity change, unneeded if you are doing a light setup from scratch using almost any recent Sollumz version.
{% endhint %}

{% hint style="info" %}
Check **Limited to Selected** to make the change to selected lights only.
{% endhint %}

#### Reload Entity Sets

It reloads old entity sets from older MLOs projects before the last entity set system update.

{% hint style="info" %}
Only needed if you are migrating an old MLO project to the newer Entity Sets system, not needed anymore if you are working on the latest Sollumz version in a new MLO project.
{% endhint %}
