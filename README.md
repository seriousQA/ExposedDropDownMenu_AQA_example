# ExposedDropdownMenu_AQA_example
Example of ExposedDropdownMenu (material3:1.4.0-alpha13) for test automation

![Kotlin](https://img.shields.io/badge/kotlin-%237F52FF.svg?style=for-the-badge&logo=kotlin&logoColor=white) 	![Android Studio](https://img.shields.io/badge/Android_Studio-3DDC84?style=for-the-badge&logo=android-studio&logoColor=white) ![Apache-2-0](https://img.shields.io/badge/Apache--2.0-green?style=for-the-badge) ![Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=for-the-badge&logo=Jetpack%20Compose&logoColor=white) ![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)

**ExposedDropdownMenu** is a menu display a list of choices on a temporary surface. It appears when users interact with a button, action, or other control.. [dev_android_ExposedDropDownMenu](https://developer.android.com/reference/kotlin/androidx/compose/material3/package-summary#textfield)

To interact using uiautomator2 you need:
1) In  build.gradle (:app) add the UIAutomator dependency:
androidTestImplementation('androidx.test.uiautomator:uiautomator:$yourUiautomator2DriverVersion')
2) add reference on androidx.compose.ui.semantics:
import androidx.compose.ui.semantics.semantics
import androidx.compose.ui.semantics.testTagsAsResourceId
3) locate the root composable function in your UI and enable test tags by setting **testTagsAsResourceId** to true in the modifier
4) add a test tag for each composable function you need to interact with during the tests

![testTagAsResourceId](https://github.com/user-attachments/assets/a96bd6e1-8be8-489f-9ef8-80b5dd1c9613)
![ExposedDropDownMenuItems](https://github.com/user-attachments/assets/f33ab081-5c8f-491f-906b-3c5a07c5b9eb)



