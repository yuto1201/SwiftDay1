# SwiftDay1

# 🌹 3Dモデル表示アプリ - Day1

## ✅ 本日の取り組み内容
- 3Dモデル「BeautifulRose.usdz」を探して準備
- SwiftUI + SceneKit で 3Dモデルをアプリに表示

## ✅ 成果物

### 📱 3Dモデル表示画面

BeautifulRose.usdz を回転・ズームできるビューを実装しました。

<details>
<summary>📄 コードを見る</summary>

#### ContentView.swift

```swift
import SwiftUI
import SceneKit

struct ContentView: View {
    var body: some View {
        SceneView(
            scene: SCNScene(named: "BeautifulRose.usdz"),
            options: [.autoenablesDefaultLighting, .allowsCameraControl]
        )
    }
}
```


#### FlowerPomo.swift
```
import SwiftUI

@main
struct ModelViewerApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
    }
}

```
