---
description: Here you'll learn how to create a basic custom prop for GTA V.
---

# 🔮 Basic Creation

#### For a better understand about the workflow and the formats check: [Sollumz Hierarchy](../../sollum-objects/) and [YDR](../../../gta-stuff/drawables/drawable-.ydr.md)

{% hint style="info" %}
You must know Blender's basics before following this tutorial, go back to [..](../../../ "mention")to learn more.
{% endhint %}

{% hint style="info" %}
You can create your own models, buy or download them from the Internet. As long you have a textured 3d model, you will be able to work with it.
{% endhint %}

For this example, I'll be using this Sofa model.

<figure><img src="../../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

After downloading it, make sure the model's format is one of the supported formats by Blender.

#### The following are the most commonly used formats.

<table data-view="cards"><thead><tr><th></th><th align="center"></th><th></th></tr></thead><tbody><tr><td></td><td align="center">FBX</td><td></td></tr><tr><td></td><td align="center">OBJ</td><td></td></tr><tr><td></td><td align="center">DAE</td><td></td></tr><tr><td></td><td align="center">GLB/GLTF</td><td></td></tr></tbody></table>

{% hint style="info" %}
It must come with textures,`PNG`and`TGA`formats are recommended.
{% endhint %}

## Importing and preparing the model

Now import the model and the reference model.

{% hint style="info" %}
Use a scale reference model to match the game's scale, get a reference model from [here](https://cdn.discordapp.com/attachments/965904175672217640/1074571717428641792/ped\_scale.fbx).
{% endhint %}

{% hint style="info" %}
If the model comes with textures but they aren't assigned upon importing, assign them by hand.
{% endhint %}

<figure><img src="../../../.gitbook/assets/blender_w8G4TUGqgI.gif" alt=""><figcaption><p>Sofas for giants is a reality among modern societies.</p></figcaption></figure>

Do the needed transforms to get the correct scale, position and rotation.

{% hint style="info" %}
Move with G, Scale with S and Rotate with R.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (17).png" alt=""><figcaption><p>It's a fact that most people use sofas like this, right?</p></figcaption></figure>

Now go to `Object` > `Apply` > `All Transforms`, this will reset all the scale, position and scale values to avoid any possible issue during exporting.

<div align="center">

<figure><img src="../../../.gitbook/assets/blender_Z4GHI9Mdwo.gif" alt=""><figcaption></figcaption></figure>

</div>

<figure><img src="../../../.gitbook/assets/blender_E7xo7e6Bz2.gif" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
In case you know that your object's pivot location is right, just uncheck Location to keep it.
{% endhint %}

{% hint style="info" %}
Since the prop will be placeable, it should have its origin at the lowest part but also centered, however, in this case the model I chose already had this type of origin.
{% endhint %}

In case you need to change the origin, do the following:

<figure><img src="../../../.gitbook/assets/blender_F1m7dLKEWs.gif" alt=""><figcaption><p>Hi mom!</p></figcaption></figure>

&#x20;\
Now you will be able to move just the origin, to meet the lower part, you can help yourself using the snapping tools.

{% hint style="info" %}
Remember to uncheck `Affect Only: Origins` once you finish positioning the origin to your liking.
{% endhint %}

## Materials

In most of cases you don't need to manually set materials, you can convert already materials from almost any mesh by pressing `V` > `Convert Material` or by pressing `Auto Convert` button Inside `Shader Tools` > `Tools`

{% hint style="warning" %}
Please note that in any given material that your object has, its `Color Node` node **MUST** be connected to an image texture since GTA and Sollumz can't use or convert colors.
{% endhint %}

<figure><img src="../../../.gitbook/assets/blender_V4HhVB7YMa.gif" alt="" width="563"><figcaption><p>OMG, WHERE DID THE SHINE GO?</p></figcaption></figure>

{% hint style="info" %}
Just if you haven't done it already, you can safely delete the ped reference model, we don't need it anymore.
{% endhint %}

Alternatively, you can create shader materials by clicking `Convert Active Material` in case you need a very specific shader other than: `default`, `normal`, `normal_spec` or `spec`

<figure><img src="../../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
It is worth knowing that Shader Materials have some parameters that can be tweaked to get the desired look, but this will be covered in the future.
{% endhint %}

## Naming

Once we have setup all the materials as we want, we should give this Sofa a good name, please refer to [naming-conventions.md](../../../gta-stuff/naming-conventions.md "mention")to learn more.

<figure><img src="../../../.gitbook/assets/blender_58gvDoKYWe.gif" alt=""><figcaption></figcaption></figure>

## Drawable

Now it's time to turn this mesh into a usable GTA drawable.

Navigate to `Drawable Tools` > `Create Drawable Objects` > `Create Drawable Objects`

{% hint style="warning" %}
Since we are doing a prop, it needs collision, so you must check Auto-Embed collision.
{% endhint %}

<figure><img src="../../../.gitbook/assets/blender_gvI3X0kFuj.gif" alt=""><figcaption></figcaption></figure>

## Collision Materials

Let's set some proper materials to our newly created collision.

In order to work easily, we should hide the drawable geometry, usually named with a `_geom` suffix

<figure><img src="../../../.gitbook/assets/blender_GfCl38nAS6.gif" alt=""><figcaption></figcaption></figure>

Select the `Bound Poly Mesh` object, if you are working with mutiple drawables at once, you will see a `.0xx` numeric suffix

Navigate to `Collision Tools` > `Create Collision Material`

<div align="center" data-full-width="true">

<figure><img src="../../../.gitbook/assets/blender_5QtS8lXhUw.gif" alt="" width="362"><figcaption></figcaption></figure>

</div>

Go to Material Properties, there you will find your material slots

<figure><img src="../../../.gitbook/assets/blender_bldAe0mnhP.gif" alt=""><figcaption></figcaption></figure>

Since each material is assigned to a set of faces, it is possible to select them by pressing Select while in edit mode, in this case the sofa is divided into two parts, wood and leather parts, this will make it really easy to assign the right material.

<figure><img src="../../../.gitbook/assets/blender_Pl1PFj0KmI.gif" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Do not count on this for all situations, there will be situations where you will have to manually select the geometry to correctly select the parts that will belong to a certain material. You can toggle X-Ray to help yourself to do a better selection of geometry if needed.
{% endhint %}

{% hint style="info" %}
A good way to assign manually selected geometry to collision material is to create it using the **Create Collision Material** button while selecting the desired material within the Create **Collision Material** menu.
{% endhint %}
