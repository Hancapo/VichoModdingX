---
icon: gif
---

# Anims

## 🔧 Functionality

### It creates a Clip Dictionary object based on the object(s) selection.

***

#### Supported Sollum Types:

* [x] Drawable
* [x] Fragment

#### Supported Animation Types:

* [x] Object animations.
* [x] UV Animations
* [x] Player animations.

{% hint style="warning" %}
For proper UV Anims' Clip hash generation, you should at least select your `Drawable` object and use **Order Shaders** button without touching anything to update the material list.

<img src="../../../../../../.gitbook/assets/image (1).png" alt="" data-size="original">
{% endhint %}

{% hint style="info" %}
Player animations are not fully supported, if you are doing just a single animation it will work. multiple ones (more than one **NLA Tracks**) aren't supported and will be ignored.
{% endhint %}
