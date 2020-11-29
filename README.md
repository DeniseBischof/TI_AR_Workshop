**TI Workshop Augmented Reality**

Denise Bischof | denise.bischof@filmuniversitaet.de | Film University Babelsberg _KONRAD WOLF_

---

# Augmented Reality in Unity

-   [Augmented Reality in Unity](#AugmentedRealityinUnity)
    -   [Basics](#Basics)
        -   [Unity](#Unity)
        -   [Vuforia](#Vuforia)
        -   [ARFoundation](#ARFoundation)
    -   [Example projects](#Example-projects)

---

## Basics

### Unity
Unity is a cross-platform game engine developed by Unity Technologies, first announced and released in June 2005 at Apple Inc.'s Worldwide Developers Conference as a Mac OS X-exclusive game engine. As of 2018, the engine had been extended to support more than 25 platforms. The engine can be used to create three-dimensional, two-dimensional, virtual reality, and augmented reality games, as well as simulations and other experiences. The engine has been adopted by industries outside video gaming, such as film, automotive, architecture, engineering and construction. 
[Download Unity](https://unity3d.com/get-unity/download)

Unity Interface: 

Unity gives users the ability to create games and experiences in both 2D and 3D, and the engine offers a primary scripting API in C#, for both the Unity editor in the form of plugins, and games themselves, as well as drag and drop functionality.

Here is an example for C# code:
```C#
public class Movement : MonoBehaviour {
   public float speed;
   
   void Update() {
   float h = Input.GetAxisRaw(“Horizontal”);
   float v = Input.GetAxisRaw(“Vertical”);
   
   gameObject.transform.position = new Vector2 (transform.position.x + (h * speed), 
      transform.position.y + (v * speed));
   }
}

```

This is a simple movement input script in C# for Unity.


### Vuforia
Vuforia is an augmented reality software development kit (SDK) for mobile devices that enables the creation of augmented reality applications.[1] It uses computer vision technology to recognize and track planar images and 3D objects in real time. 

This image registration capability enables developers to position and orient virtual objects, such as 3D models and other media, in relation to real world objects when they are viewed through the camera of a mobile device. The virtual object then tracks the position and orientation of the image in real-time so that the viewer's perspective on the object corresponds with the perspective on the target. It thus appears that the virtual object is a part of the real-world scene. 



### ARFoundation


## Example projects

To get a first idea of what Three.js can do, let's have a look at some example projects:

-   [PharaosAR](https://unity.com/de/madewith/pharos-ar) <br><img src="https://unity.com/sites/default/files/styles/16_9_xl/public/2019-04/pharos-ar-hero-1920x1000.jpg?itok=IJ0rQtOV" width="400">


## References

[[1] Unity definition](https://unity.com/de/products/unity-platform)

[[2] Vuforia definition](https://library.vuforia.com/getting-started/overview.html)

[[3] ARFoundation definition](https://unity.com/unity/features/arfoundation)

---

The End

💻 💫🔺
