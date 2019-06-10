Twisted Terrace Tiny DOTS Edition
=================================

This project serves as a translation between the Game Object-based Unity and the
new DOTS (ECS) project style.

Installing
----------

You will need the latest version of **Unity 2019.2**, which is in beta at the
time of writing.

Once you have installed Unity and cloned the project, open the project through
Unity Hub. This process will take a while.

You will eventually see an Editor Layout like this:

![](media/e608bd8c06dda533254b86155ba85254.png)

Contributing Checklist
----------------------

### Add Sprite Assets to the Project

Normal rules for importing sprites applies here.

### Add Text to the UICanvas

I have created an example entity with text as a child of the UICanvas. You can
create a new entity using the Entity menu at the top. Then add the necessary
components.

If you would like to use a custom font, you will need to create it using
TextMeshPro. This guide will walk you through the process:
<http://digitalnativestudios.com/textmeshpro/docs/font/>

**Set the Render Mode to SMOOTH_HINTED!**

There are other components you can add to the text. You can find documentation
for them here:
<https://docs.unity3d.com/Packages/com.unity.tiny@0.15/manual/module-text.html>

### Add Sprites with Animations

You can right click on the prefabs scene to make it the active scene. When you
do so, creating new entities adds them to the scene. See if you can figure out
how to make your sprites animated.

Missing Features
----------------

Some features were removed when Tiny merged with DOTS C\#. I expect the features
will be added back over time. If the above items are completed before the
missing features are added, we may attempt to implement the missing features.

### Tilemaps

It seems we can still create tiles, but we can’t place them in a tilemap yet. It
would be relatively straightforward to render a tilemap given a 2D image of tile
indices and an array of tiles.

### Physics

Physics is gone at the moment. If I get my 3D physics working before 2D physics
gets implemented we can use that.
