## Landmarks Recognition App
1/ ![Screenshot_20240814-154013](https://github.com/user-attachments/assets/7eba6307-c780-4cf9-b1b0-5e38d43a2088)
2/ ![Screenshot_20240814-153954](https://github.com/user-attachments/assets/5f07c08b-2c75-49b6-bb1b-a75986219ef8)
3/ ![Screenshot_20240814-154257](https://github.com/user-attachments/assets/240f8569-0518-4433-9681-5d67b7ec7d88)
4/ ![Screenshot_20240814-154341](https://github.com/user-attachments/assets/c111b3d9-990e-4597-86ae-44854ff869f7)



This project is an Android application designed to recognize landmarks using a TensorFlow Lite model. The app leverages the camera to capture images and classify them in real-time, providing users with the name and confidence score of the recognized landmarks.

### Features

- **Real-time Landmark Recognition**: Utilizes the device's camera to capture and classify landmarks in real-time.
- **TensorFlow Lite Integration**: Employs a pre-trained TensorFlow Lite model (`landmarks.tflite`) for efficient and accurate landmark classification.
- **User-Friendly Interface**: Displays classification results with a clean and intuitive UI using Jetpack Compose.
- **CameraX Integration**: Uses CameraX for camera functionalities, ensuring compatibility and ease of use.

### Technologies Used

- **Kotlin**: Primary programming language for the app.
- **TensorFlow Lite**: For on-device machine learning and landmark classification.
- **Jetpack Compose**: For building the UI.
- **CameraX**: For camera functionalities.
- **Gradle**: For project build and dependency management.

### Project Structure

- **`MainActivity.kt`**: The main entry point of the app, handling camera permissions and setting up the UI.
- **`TfLiteLandmarkClassifier.kt`**: Implements the `LandmarkClassifier` interface using TensorFlow Lite for landmark classification.
- **`LandmarkImageAnalyzer.kt`**: Analyzes camera frames and uses the classifier to recognize landmarks.
- **`Classification.kt`**: Data class representing the classification result.
- **`CameraPreview.kt`**: Composable function to display the camera preview using CameraX.
- **`BitmapExt.kt`**: Extension function for Bitmap to perform center cropping.
- **`AndroidManifest.xml`**: Declares app permissions and main activity.

### Getting Started

1. **Clone the repository**:
    ```sh
    git clone https://github.com/Tharwat07/Landmarks-android.git
    cd landmarks-recognition-app
    ```

2. **Open the project in Android Studio**.

3. **Build and run the app** on an Android device with camera permissions enabled.

### Acknowledgements

- The TensorFlow Lite model used in this project is pre-trained and optimized for on-device inference.
- Special thanks to the TensorFlow team for providing robust tools and libraries for machine learning.
- This project is an exercise from the YouTube channel by Phlipe.

### License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
