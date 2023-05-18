# ApplicationLifeCycle
Understanding iOS Application Life Cycle

```
import UIKit

class SceneDelegate: UIResponder, UIWindowSceneDelegate {
    var window: UIWindow?
    func scene(_ scene: UIScene, willConnectTo session: UISceneSession, options connectionOptions: UIScene.ConnectionOptions) {
        //called when the app initially starts.
        guard let _ = (scene as? UIWindowScene) else { return }
        print(#function)
    }
    func sceneDidDisconnect(_ scene: UIScene) {
        // Called as the scene is being released by the system. (app closed)
        // This occurs shortly after the scene enters the background, or when its session is discarded.
        // Release any resources associated with this scene that can be re-created the next time the scene connects.
        // The scene may reconnect later, as its session was not necessarily discarded (see `application:didDiscardSceneSessions` instead).
        print(#function)
    }
    func sceneDidBecomeActive(_ scene: UIScene) {
        // Called when the scene has moved from an inactive state to an active state.
        // Use this method to restart any tasks that were paused (or not yet started) when the scene was inactive.
        print(#function)
    }
    func sceneWillResignActive(_ scene: UIScene) {
        // Called when the scene will move from an active state to an inactive state.
        // This may occur due to temporary interruptions (ex. an incoming phone call).
        print(#function)
    }
    func sceneWillEnterForeground(_ scene: UIScene) {
        // Called as the scene transitions from the background to the foreground.
        // Use this method to undo the changes made on entering the background.
        print(#function)
    }
    func sceneDidEnterBackground(_ scene: UIScene) {
        // Called as the scene transitions from the foreground to the background.
        // Use this method to save data, release shared resources, and store enough scene-specific state information
        // to restore the scene back to its current state.
        print(#function)
    }
}
```

Above are various states of application life cycle.

<img width="771" alt="applifecycle" src="https://github.com/aparth443/ApplicationLifeCycle/assets/112768328/93bcc709-b631-44dc-ad9a-0d61776e6a24">


