# 🫑 Drawable Model

## Specification

A [Drawable Model](drawable-model.md) is an object derived from [Drawable](drawable.md) whose function is to package the geometry.

## Parameters

| Parameter                  | Meaning                                                                                                        |
| -------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `Render Mask`              | Unknown behavior, it could have something to do with render order. If unsure leave it as `255`                 |
| `Unknown 1 (Hidden in UI)` | Bones count if the Drawable has a skeleton.                                                                    |
| `Flags (Hidden in UI)`     | It has relation with certain behaviors, if unsure leave it as 0                                                |
| `LOD Level (Hidden in UI)` | <p>What LOD level is going to be used.<br><code>High > Medium > Low > Vlow</code> are available to choose.</p> |

{% hint style="info" %}
The hidden parameters are automatically calculated upon export.
{% endhint %}

{% hint style="warning" %}
This object MUST have a [Drawable](drawable.md) as parent in any given circumstance.
{% endhint %}

{% hint style="success" %}
A [Drawable](drawable.md) can have almost any number of [Drawable Models](drawable-model.md).
{% endhint %}
