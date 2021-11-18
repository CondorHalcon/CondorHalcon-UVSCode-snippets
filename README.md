# CH Unity VSCode Snippets

Unity VSCode Snippets is a Unity C# snippet extention built for VSCode.

Author: [@CondorHalcon](https://github.com/CondorHalcon)

### Contents
- [Features](#features)
- [Requirments](#requirements)
- [Known Issues](#known-issues)
- [Release Notes](#release-notes-v100-alpha1---2021-02-13)

## Features
### Assemblies
Name | Prefix
-----|-------
UnityEditor | `using UnityEditor;`
UnityEngine.CoreModule | `using UnityEngine;`
UnityEngine.UIModule | `using UnityEngine.UI;`
### UnityEngine.CoreModule
#### Attributes
Name | Prefix
-----|-------
HeaderAttribute | `[Header("header")]`
HideInInspector  | `[HideInInspector]`
RangeAttribute | `[Range(x,y)]`
SerializeField | `[SerializeField]`
TooltipAttribute | `[Tooltip("tooltip")]`
#### Component class
Name | Prefix
-----|-------
Component.gameObject | `gameObject`
Component.tag | `tag`
Component.transform | `transform`
Component.BroadcastMessage | `BrodacastMessage(string methodName, object parameter, SendMessageOptions options)`, `BrodacastMessage(string methodName,SendMessageOptions options)`
Component.CompareTag | `CompareTag(string tag)`
Component.GetComponent | `GetComponent(Type type)`, `GetComponent<Type type>()`, `GetComponent(string type)`
Component.GetComponentInChildren | `GetComponentInChildren(Type type)`, `GetComponentInChildren<Type type>()`
Component.GetComponentInParent | `GetComponentInParent(Type type)`, `GetComponentInParent<Type type>()`
Component.GetComponents | `GetComponents(Type type)`, `GetComponents<Type type>()`
Component.GetComponentsInChildren | `GetComponentsInChildren(Type type, bool includeInactive)`, `GetComponentsInChildren<${1:Type type}>(${1:bool includeInactive})`
Component.GetComponentsInParent | `GetComponentsInParent(Type t, bool includeInactive)`, `GetComponentsInParent<Type type>()`, `GetComponentsInParent<Type type>(bool includeInactive)`
Component.SendMessage | `SendMessage(string methodName)`, `SendMessage(string methodName, object value)`, `SendMessage(string methodName, object value, SendMessageOptions options)`, `SendMessage(string methodName,SendMessageOptions options)`
Component.SendMessageUpwards | `SendMessageUpwards(string methodName, SendMessageOptions options)`, `SendMessageUpwards(string methodName, object value, SendMessageOptions options)`
Component.TryGetComponent | `TryGetComponent(Type type, out Component component)`, `TryGetComponent(out Component component)`
#### Object class
Name | Prefix
-----|-------
Object.hideFlags | `hideFlags`
Object.name | `name`
Object child class | `class Object`
Object.GetInstanceID | `GetInstanceID()`
Object.ToString | `ToString()`
Object.Destroy | `Object.Destroy`
Object.DestroyImmediate | `DestroyImmediate(Object obj, bool allowDestroyingAssets = false);`
Object.DontDestroyOnLoad | `DontDestroyOnLoad(Object target);`
Object.FindObjectOfType | `FindObjectOfType(Type type)`, `FindObjectOfType<type>()`
Object.FindObjectsOfType | `FindObjectsOfType(Type type)`, `FindObjectsOfType<Type type>()`
Object.Instantiate | `Instantiate(Object original);`, `Instantiate(Object original, Transform parent);`, `Instantiate(Object original, Transform parent, bool instantiateInWorldSpace);`, `Instantiate(Object original, Vector3 position, Quaternion rotation);`, `Instantiate(Object original, Vector3 position, Quaternion rotation, Transform parent);`

## Requirements
item | Minimum | Recomended
-------|---------|-----------
VSCode | 1.53.0  | 1.53.0
Unity  | -       | 2019.4LTS

## Known Issues
None

## Release Notes [v1.2.0-alpha]
> All [changelogs](https://github.com/CondorHalcon/CH-UnityVSCode-Snippets/CHANGELOG.md).

### Added
- Attributes
  - HeaderAttribute `[Header(header)], []`
  - HideInInspector `[HideInInspector], []`
  - RangeAttribute `[Range(x,y)], []`
  - SerializeField `[SerializeField], []`
  - TooltipAttribute `[Tooltip(tooltip)], []`
- Component class
  - Component.gameObject `gameObject`
  - Component.tag `tag`
  - Component.transform `transform`
  - Component.BroadcastMessage
    - `BrodacastMessage(string methodName, object parameter, SendMessageOptions options)`
    - `BrodacastMessage(string methodName,SendMessageOptions options)`
  - Component.CompareTag `CompareTag(string tag)`
  - Component.GetComponent
    - `GetComponent(Type type)`
    - `GetComponent<Type type>()`
    - `GetComponent(string type)`
  - Component.GetComponentInChildren
    - `GetComponentInChildren(Type type)`
    - `GetComponentInChildren<Type type>()`
  - Component.GetComponentInParent
    - `GetComponentInParent(Type type)`
    - `GetComponentInParent<Type type>()`
  - Component.GetComponents
    - `GetComponents(Type type)`
    - `GetComponents<Type type>()`
  - Component.GetComponentsInChildren
    - `GetComponentsInChildren(Type type, bool includeInactive)`
    - `GetComponentsInChildren<${1:Type type}>(${1:bool includeInactive})`
  - Component.GetComponentsInParent
    - `GetComponentsInParent(Type t, bool includeInactive)`
    - `GetComponentsInParent<Type type>()`
    - `GetComponentsInParent<Type type>(bool includeInactive)`
  - Component.SendMessage
    - `SendMessage(string methodName)`
    - `SendMessage(string methodName, object value)`
    - `SendMessage(string methodName, object value, SendMessageOptions options)`
    - `SendMessage(string methodName,SendMessageOptions options)`
  - Component.SendMessageUpwards
    - `SendMessageUpwards(string methodName, SendMessageOptions options)`
    - `SendMessageUpwards(string methodName, object value, SendMessageOptions options)`
  - Component.TryGetComponent
    - `TryGetComponent(Type type, out Component component)`
    - `TryGetComponent(out Component component)`
### Removed
- Assemblies
  - UnityEngine.AIModule assembly `using UnityEngine.AI;`
  - UnityEngine.AndroidJNIModule assembly `using UnityEngine.AndroidJNI;`
  - UnityEngine.AnimationModule assembly `using UnityEngine.Animation;`
  - UnityEngine.AssetBundleModule assembly `using UnityEngine.AssetBundle;`
  - UnityEngine.AudioModule assembly `using UnityEngine.Audio;`
  - UnityEngine.ClothModule assembly `using UnityEngine.Cloth;`
  - UnityEngine.DirectorModule assembly `using UnityEngine.Director;`
  - UnityEngine.GameCenterModule assembly `using UnityEngine.GameCenter;`
  - UnityEngine.ImageConversionModule assembly `using UnityEngine.ImageConversion;`
  - UnityEngine.IMGUIModule assembly `using UnityEngine.IMGUI;`
  - UnityEngine.InputLegacyModule assembly `using UnityEngine.InputLegacy;`
  - UnityEngine.JSONSerializeModule assembly `using UnityEngine.JSONSerialize;`
  - UnityEngine.ParticleSystemModule assembly `using UnityEngine.ParticleSystem;`
  - UnityEngine.Physics2D assembly `using UnityEngine.Physics2D;`
  - UnityEngine.PhysicsModule assembly `using UnityEngine.Physics;`
  - UnityEngine.ScreenCaptureModule assembly `using UnityEngine.ScreenCapture;`
  - UnityEngine.SharedInternalsModule assembly `using UnityEngine.SharedInternals;`
  - UnityEngine.SubsystemsModule assembly `using UnityEngine.Subsystems;`
  - UnityEngine.TerrainModule assembly `using UnityEngine.Terrain;`
  - UnityEngine.TerrainPhysicsModule assembly `using UnityEngine.TerrainPhysics;`
  - UnityEngine.TextRenderingModule assembly `using UnityEngine.TextRendering;`
  - UnityEngine.TilemapModule assembly `using UnityEngine.Tilemap;`
  - UnityEngine.UIElementsModule assembly `using UnityEngine.UIElements;`
  - UnityEngine.UmbraModule assembly `using UnityEngine.Umbra;`
  - UnityEngine.UnityAnalyticsModule assembly `using UnityEngine.UnityAnalytics;`
  - UnityEngine.UnityWebRequestAssetBundleModule assembly `using UnityEngine.UnityWebRequestAssetBundle;`
  - UnityEngine.UnityWebRequestAudioModule assembly `using UnityEngine.UnityWebRequestAudio;`
  - UnityEngine.UnityWebRequestModule assembly `using UnityEngine.UnityWebRequest;`
  - UnityEngine.UnityWebRequestTextureModule assembly `using UnityEngine.UnityWebRequestTexture;`
  - UnityEngine.UnityWebRequestWWWModule assembly `using UnityEngine.UnityWebRequestWWW;`
  - UnityEngine.VehiclesModule assembly `using UnityEngine.Vehicles;`
  - UnityEngine.VideoModule assembly `using UnityEngine.Video;`
  - UnityEngine.VRModule assembly `using UnityEngine.VR;`
  - UnityEngine.WebGLModule assembly `using UnityEngine.WebGL;`
  - UnityEngine.WindModule assembly `using UnityEngine.Wind;`
  - UnityEngine.XRModule assembly `using UnityEngine.XR;`
- Object class
  - Object child class `class Object`
