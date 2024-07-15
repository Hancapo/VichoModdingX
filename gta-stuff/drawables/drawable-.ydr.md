# 🍓 Drawable (.YDR)

## **Specification**

A [Drawable](../../sollumz/sollum-objects/drawable.md) is the file type used for map models, vegetation and weapons in GTA V.

<figure><img src="../../.gitbook/assets/image (23).png" alt=""><figcaption><p>ss1_03_north.ydr</p></figcaption></figure>

## Features/Support

|                   |    |
| ----------------- | -- |
| Lights            | 🟩 |
| Geometry          | 🟩 |
| Embedded Textures | 🟩 |
| Physics           | 🟧 |
| Skeleton          | 🟩 |

{% hint style="info" %}
YDR objects can have physics, but it cannot be used to create breakable objects or animated objects with collision, use YFTs instead.
{% endhint %}

## Sollumz Hierarchy

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption><p>An example of a YDR with two drawable models and two drawable geometry per model.</p></figcaption></figure>

### It uses [Drawable](../../sollumz/sollum-objects/drawable.md), [Drawable Model](../../sollumz/sollum-objects/drawable-model.md) and [Drawable Geometry](broken-reference) Sollum objects.
