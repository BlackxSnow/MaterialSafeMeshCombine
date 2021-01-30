# MaterialSafeMeshCombine
Rewrite of [this script](http://answers.unity.com/answers/1123487/view.html) for neatness, safety, and functionality. Combines meshes in UnityEngine accounting for materials.

# Usage
Download or copy the script into your project. At the top of the script you want to use this with, use the namespace ("using Utility"). This method is an extension of GameObject, and thus you can simply call gameObject.MeshCombine().

You can optionally include a GameObject[] or multiple GameObject variables as parameters to ignore these in the combining.

# Notes
- This works whether the calling GameObject is part of the combined mesh or an empty parent.
- destroyObjects preserve their children as children of the calling GameObject.
- Any children of ignored GameObjects will also be ignored.
