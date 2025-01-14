# Camera Shake Controller  
A Unity script designed to add shake effects to your camera, enhancing the player's experience by creating dynamic camera movements. It is ideal for simulating impacts, explosions, or other dramatic moments in your game.

## Features  
- **Shake Effects**: Adds camera shake effects when triggered, adding intensity and immersion to the gameplay.  
- **Customizable Parameters**: Easily control the shake intensity, duration, and frequency to match the desired effect.  
- **Simple Integration**: Just import the `CameraShakeController` package, attach the script to your camera, and you're ready to create dynamic shake effects with minimal setup.  
- **Triggerable Events**: Control the shake through code, making it easy to activate during specific events like collisions, explosions, or key actions in the game.

## Installation  
1. Download the [`CameraShakeController.unitypackage`](CameraShakeController.unitypackage) file from this repository.  
2. Open your Unity project and go to **Assets > Import Package > Custom Package**.  
3. Select the `CameraShakeController.unitypackage` file and click **Import**.  
4. After importing, attach the `CameraShakeController` script to your main camera in the scene.  
   - **Important**: Ensure that the camera's position is not controlled by another script (such as a camera follow script) to prevent the shake effect from being canceled or overridden.  

## How to Use  
1. Import the asset by following the installation steps above.  
2. Attach the `CameraShakeController` script to your camera by selecting the camera in the scene and clicking **Add Component**.  
3. Adjust the script parameters in the **Inspector** to customize the shake effect (e.g., intensity, duration, frequency).  
4. To trigger the camera shake:
   - Call the `TriggerShake()` method from your other scripts when you want the shake effect to occur.
   - Example:
     ```csharp
     CameraShakeController.TriggerShake(0.3f, 0.5f); // Shake with duration 0.3 seconds and magnitude 0.5.
     ```

## License  
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
