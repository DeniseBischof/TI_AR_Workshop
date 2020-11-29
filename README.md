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

<img src="https://raw.githubusercontent.com/DeniseBischof/TI_AR_Workshop/main/Pictures/Unity_Interface.png" width="600">

**1: Hierarchy** <br>
The Hierarchy window contains a list of every GameObject in the current Scene. Some of these are direct instances of Asset files (like 3D models), and others are instances of Prefabs, which are custom GameObjects that make up most of your game. When you add or remove GameObjects the Scene, they appear and disappear from the Hierarchy as well. 

**2: Scene** <br>
The Scene view is your interactive view into the world you are creating. You can use the Scene view to select and position scenery, characters, Cameras, lights, and all other types of GameObjects. Selecting, manipulating, and modifying GameObjects in the Scene view are some of the first skills you must learn to begin working in Unity.

**3: Project window** <br>
The Project window displays all of the files related to your Project and is the main way you can navigate and find Assets and other Project files in your application. When you start a new Project by default this window is open. However, if you cannot find it, or it is closed, you can open it via Window > General > Project or use the keyboard command Ctrl + 9 (Command + 9 on macOS).

**4: Inspector** <br>
Projects in the Unity Editor are made up of multiple GameObjects that contain scripts, sounds, Meshes, and other graphical elements such as Lights. The Inspector window displays detailed information about the currently selected GameObject, including all attached components and their properties, and allows you to modify the functionality of GameObjects in your Scene.

**The Toolbar** at the top provides access to the most essential working features. On the left it contains the basic tools for manipulating the Scene view and the GameObjects within it. In the centre are the play, pause and step controls. The buttons to the right give you access to Unity Collaborate, Unity Cloud Services and your Unity Account, followed by a layer visibility menu, and finally the Editor layout menu (which provides some alternate layouts for the Editor windows, and allows you to save your own custom layouts).


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
Vuforia is an augmented reality software development kit (SDK) for mobile devices that enables the creation of augmented reality applications. It uses computer vision technology to recognize and track planar images and 3D objects in real time. 

<img src="https://raw.githubusercontent.com/DeniseBischof/TI_AR_Workshop/main/Pictures/Vuforia_3DObj_Ex.png" height="175">

This image registration capability enables developers to position and orient virtual objects, such as 3D models and other media, in relation to real world objects when they are viewed through the camera of a mobile device. The virtual object then tracks the position and orientation of the image in real-time so that the viewer's perspective on the object corresponds with the perspective on the target. It thus appears that the virtual object is a part of the real-world scene. 

<img src="https://raw.githubusercontent.com/DeniseBischof/TI_AR_Workshop/main/Pictures/Feature_Ex.png" width="400">



### ARFoundation

AR Foundation allows you to work with augmented reality platforms in a multi-platform way within Unity. This package presents an interface for Unity developers to use, but doesn't implement any AR features itself. To use AR Foundation on a target device, you also need separate packages for the target platforms officially supported by Unity:

AR Foundation includes core features from ARKit, ARCore, Magic Leap, and HoloLens, as well as unique Unity features to build robust apps that are ready to ship to internal stakeholders or on any app store. This framework enables you to take advantage of all of these features in a unified workflow.

<img src="https://unity.com/sites/default/files/styles/16_9_s_scale_width/public/2020-06/AR%20Foundation%202.1%20Chart%20%282019%20LTS%29.png?itok=hPpyk6_6" width="600">

**ARCore Point Cloud:** <br>
<img src="https://miro.medium.com/max/2048/1*g3vFBvvBOjM9Hk5aPyrO2w.jpeg" width="600">



[ARFoundation Samples](https://github.com/Unity-Technologies/arfoundation-samples)

## Example projects

To get a first idea of what Three.js can do, let's have a look at some example projects:

-   [PharaosAR](https://unity.com/de/madewith/pharos-ar) 
<br><img src="https://unity.com/sites/default/files/styles/16_9_xl/public/2019-04/pharos-ar-hero-1920x1000.jpg?itok=IJ0rQtOV" width="400">


## References

[[1] Unity definition](https://unity.com/de/products/unity-platform)

[[2] Vuforia definition](https://library.vuforia.com/getting-started/overview.html)

[[3] ARFoundation definition](https://unity.com/unity/features/arfoundation)

---

The End
