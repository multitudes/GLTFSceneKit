# GLTFSceneKit
glTF loader for SceneKit (swift)

![ScreenShot](https://raw.githubusercontent.com/rooom-com/GLTFSceneKit/master/screenshot.png)

## Installation
### Using [CocoaPods](http://cocoapods.org/)

Add the following to your [Podfile](http://guides.cocoapods.org/using/the-podfile.html):

```rb
pod 'GLTFSceneKit', :git => 'https://github.com/rooom-com/GLTFSceneKit.git'
```

## Usage

### Swift
```
import GLTFSceneKit

var scene: SCNScene
do {
  let sceneSource = try GLTFSceneSource(named: "art.scnassets/Box/glTF/Box.gltf")
  scene = try sceneSource.scene()
} catch {
  print("\(error.localizedDescription)")
  return
}
```

## See also

[GLTFQuickLook](https://github.com/magicien/GLTFQuickLook) - QuickLook plugin for glTF files
