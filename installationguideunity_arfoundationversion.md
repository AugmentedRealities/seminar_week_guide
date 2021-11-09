# InstallationGuideUnity\_ARFoundationVersion

## **Unity Installation** <a href="_toc85493401" id="_toc85493401"></a>

We will use Unity 3D to develop the Android application. You can download it free from:

[**https://unity3d.com/get-unity/download**](https://unity3d.com/get-unity/download)

### Step 1 – Download and install Unity Hub <a href="_toc85493402" id="_toc85493402"></a>

We will first install the Unity Hub, which will allow us to install Unity and associated packages later.

![](.gitbook/assets/0)

Download Unity Hub from Unity 3D

Download the installer for windows. Execute the **.exe** file, agree on the Unity Terms and install Unity Hub.

### Step 2 – Create a Unity ID <a href="_toc85493403" id="_toc85493403"></a>

Go to unity3d.com and click on the right to create a Unity ID

![](<.gitbook/assets/1 (4)>)

### Step 3 – Activate Unity <a href="_toc85493404" id="_toc85493404"></a>

Open Unity Hub and click on manual activation (1). Click on Save license Request (2) and then click on license.unity3d.com/manual (3)

![](<.gitbook/assets/2 (3)>)

If necessary, sign into your Unity ID and click again on license.unity3d.com/manual:

![](.gitbook/assets/3)

This window should open, and you should upload the license request file you saved before:

![](<.gitbook/assets/4 (4)>)

Choose as a license option: Unity Personal Edition > I don't use Unity in a professional capacity:

![](.gitbook/assets/5)

Download the license file and upload it in the Unity Hub:

![](<.gitbook/assets/6 (3)>)

Now we are ready to install unity!

### Step 4 – Install Unity 2020.3.19f1 and necessary Modules <a href="_toc85493405" id="_toc85493405"></a>

In the Unity Hub click “Installs” and click on **ADD** and select** Unity 2020.3.19f1**. This is the version we will work with. Do not download or install any updates as the seminar week will be based on exactly this version.

![](<.gitbook/assets/7 (4)>)

Select the version **Unity 2020.3.19f1 **and click **Next**.![](<.gitbook/assets/8 (3)>)

If you don't see it - click on download archive:

![](<.gitbook/assets/9 (1)>)

Click on Unity Hub:

![](.gitbook/assets/10)

In the following window, select the following additional packages.

1. **Microsoft Visual Studio Community**
2. **Android Build Support:**

**1.1) Android SDK & NDK Tools,**

**1.2) Open JDK**

1. **iOS Build Support**
2. **Universal Windows Platform Build Support**
3. **Windows Build Support (IL2CPP)**
4. **Documentation**

![](<.gitbook/assets/11 (4)>) ![](.gitbook/assets/12) ![](<.gitbook/assets/13 (2)>) ![](<.gitbook/assets/14 (1)>) ![](<.gitbook/assets/15 (3)>)

Selection Window Unity Installer

The installation will take a while. After completion, you should see the** Unity Version 2020.3.19f1 **and** Android** installed.

![](.gitbook/assets/16)

Selection Window Unity Installer

### **Quick Start to AR Foundation** <a href="_toc85493406" id="_toc85493406"></a>

Unity's [AR Foundation](https://unity.com/unity/features/arfoundation) is a cross-platform framework that allows you to write augmented reality experiences once, then build for either Android or iOS devices without making any additional changes. The framework is available via Unity's AR Foundation package. ARCore's optional [ARCore Extensions for AR Foundation](https://developers.google.com/ar/develop/unity-arf/getting-started-extensions) package adds additional functionality.

1. **Hardware:**

* **ARCore** [supported device](https://developers.google.com/ar/discover/supported-devices) /** ANDROID PHONE**
  * [https://developers.google.com/ar/discover/supported-devices#android\_play](https://developers.google.com/ar/discover/supported-devices#android\_play)
* **USB cable** to connect the device to your development machine

ARCore Supported Devices will be provided during the Seminar Week, but you can still do the rest of the installation steps. Running and building a sample app will happen on DAY 1 of the Seminar Week.

We will use **Unity 3D **to develop the Android – based augmented reality apps.

### **Open Unity and install the packages** <a href="_toc85493407" id="_toc85493407"></a>

### Step 1 - Create a folder structure for the Seminar Week <a href="_toc85493408" id="_toc85493408"></a>

![](<.gitbook/assets/17 (2)>)

Folder on the desktop where all seminar week related work will be stored

### Step 2 - Open Unity and create a new 3D project <a href="_toc85493409" id="_toc85493409"></a>

In Unity Hub, go to “**Projects**” and click **NEW**, to create a new project.

![](<.gitbook/assets/18 (3)>)

You can _name_ the project as you prefer. Make sure the** Template** is set to **3D** and define a **Location** for your project. The Location would be the folder we created in the previous step. Click on “**Create**”, to create the project. This might take a while, depending on the speed of your computer.

![](.gitbook/assets/19)

### **Install Packages** <a href="_toc85493410" id="_toc85493410"></a>

### Install AR Foundation Package <a href="_toc85493411" id="_toc85493411"></a>

Select **Window > Package Manager**

![](<.gitbook/assets/20 (3)>)

In the Package Manager, from the “Packages” dropdown Menu, select “**Unity Registry”**

In the search bar, type** "AR Foundation" (1)** and click** Install (2).**

**1**

**2**

### Install ARCore XR Plugin <a href="_toc85493412" id="_toc85493412"></a>

The [ARCore XR Plugin](https://docs.unity3d.com/Packages/com.unity.xr.arcore@4.2/manual) package allows you to build augmented reality apps for Android devices. Follow these steps to install it in your Unity project if your application targets Android devices. Use the same version as the _AR Foundation_ package to avoid any compatibility issues.

Next to **Packages**, select **Unity Registry**.\
\


In the search bar, type "ARCore XR plugin".\


Select the desired version and click **Install**

In the Package Manager Window, click the  button and choose the “**Add package from git URL…**” option from the drop-down menu.

Paste the following URL into the text field:

**https://github.com/google-ar/arcore-unity-extensions.git**

Click **Add**.

You should be able to see the ARCore Extensions installed.

### **Configure Project Settings** <a href="_toc85493413" id="_toc85493413"></a>

### Step 1 - Configure Build Settings: <a href="_toc85493414" id="_toc85493414"></a>

Go to **File > Build Settings** to open the [Build Settings](https://docs.unity3d.com/Manual/BuildSettings.html) window.

Select** Android **(1) and click **Switch Platform **(2)

**1**

**2**

### Step 2 - Configure Player Settings: <a href="_toc85493415" id="_toc85493415"></a>

In the same window (**Build Settings**), click on “**Player Settings**”.

In the **Settings** window, configure the following:\
Go to **Player > Other Settings**\


Go to **Player > Other Settings > Rendering**

\
Make sure “**Auto Graphics API**” is unchecked and** remove Vulkan** as Graphics API , by clicking on it and then clicking on the minus ( **- **) symbol. Change _Color Space_ to** “Linear”**

* Go to **Player > Other Settings > Package Name**

Create a unique app ID using a **Java **package name format.\
For example, use **com.eth.AR **(1)

* Go to **Player > Other Settings > Minimum API Level**

Select **Android 7.0 'Nougat' (API Level 24) **or higher (For [AR Optional](https://developers.google.com/ar/develop/unity/enable-arcore) apps, the Minimum API level is 14.) (2)

**1**

**2**

* Go to **Player > Other Settings > Scripting Backend**

Select **IL2CPP** instead of Mono.

* Go to **Player > Other Settings > Target Architectures**

To meet the Google Play [64-bit requirement](https://developers.google.com/ar/64bit), enable ARM64 (64-bit ARM). Leave ARMv7 (32-bit ARM) enabled to support 32-bit devices



### Step 3 - Configure Project Settings <a href="_toc85493416" id="_toc85493416"></a>

AR Foundation needs to be configured to initialize XR systems on startup.

1. Open **Edit > Project Settings... **and click on the **XR Plug-in Management** section.
2. In the Android tab, enable ARCore.



### **Configure an AR session and add AR Foundation components to your scene** <a href="_toc85493417" id="_toc85493417"></a>

A scene needs an AR session to enable [AR processes](https://developers.google.com/ar/discover/concepts), such as motion tracking, environmental understanding, and lighting estimation. You will need the following game objects to support an AR session:

* **AR Session**: Controls the lifecycle of an AR experience.
* **AR Session Origin**: Transforms AR coordinates into Unity world coordinates.

Before adding the new game objects, delete the default **Main Camera**. It will be replaced by a new **AR Camera** in the **AR Session Origin**.

Add the new AR game objects to your scene: right-click the **Hierarchy** pane and select **XR**. Add a new **AR Session** and a new **AR Session Origin** game object.

### **Enable developer options and USB debugging** <a href="_toc85493418" id="_toc85493418"></a>

_This step will be done during the Seminar Week, since ARCore supported phones will be provided. For your information, here are the necessary steps to enable the Developer Mode in an Android Device._

1. To enable developer options, tap the Build Number option **7 times**. You can find this option in one of the following locations, depending on your Android version:

* **Settings > About Phone > Build Number**

1. Return to the previous screen to find** Developer Options** near the bottom.
2. At the top of the Developer options screen, you can toggle the options **on** and off. You probably want to keep this **on**. When off, most options are disabled except those that don't require communication between the device and your development computer.
3. Enable **USB debugging.**

### **Useful Links** <a href="_toc85493419" id="_toc85493419"></a>

* Free Unity Tutorials: [https://learn.unity.com/](https://learn.unity.com)
* Unity Manual : [https://docs.unity3d.com/Manual/index.html](https://docs.unity3d.com/Manual/index.html)
* AR Foundation in Unity: [https://developers.google.com/ar/develop/unity-arf/quickstart](https://developers.google.com/ar/develop/unity-arf/quickstart)
* AR Core Overview : [https://developers.google.com/ar/develop](https://developers.google.com/ar/develop)
* Unity Asset Store: [https://assetstore.unity.com/](https://assetstore.unity.com) _//You can make an account and download numerous packages and assets to use during development._
