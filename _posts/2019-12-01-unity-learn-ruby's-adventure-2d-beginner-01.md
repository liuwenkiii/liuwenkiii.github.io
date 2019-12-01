---
layout: post
title: Unity Learn  - [01] Ruby's Adventure 2D Beginner
categories: [Unity Learn, 个人翻译]
description: some word here
keywords: unity, 2D, game
---

_原文链接：https://learn.unity.com/tutorial/setting-up-the-unity-editor?language=en&projectId=5c6166dbedbc2a0021b1bc7c#_ 

# 01 - 配置 Unity Editor
_Tutorial · Beginner · 时长 20 分钟_ 

## 1.更新你的Unity 版本
在开始本教学项目之前，您需要：
- 下载 [Unity Hub](https://unity3d.com/get-unity/download)
- 下载最新的 [Unity Personal](https://store.unity.com/download?ref=personal) 官方正式版
- 用您的 Unity ID 登录
- 使用默认选项安装 Unity Editor

关于 **Unity Hub** 的使用建议，请参照 [Unity Hub documentation](https://docs.unity3d.com/Manual/GettingStartedInstallingHub.html) 

**注意：** Ruby’s Adventure: 2D Beginner 项目和配套教学内容最小只兼容至版本 2018.3，请使用大于这个版本的 Unity Editor 打开本项目。

## 2.下载 Ruby’s Adventure: 2D Beginner 项目 
请依照以下步骤下载 Ruby’s Adventure: 2D Beginner： 

1.打开 **Unity Hub** 

2.选择左侧窗口的 **学习(Learn)** 选项卡 

![learn](https://connect-cdn-prd-cn.unitychina.cn/20190829/learn/images/0e883ab9-775f-4f7e-8721-b80edd7c92f5_Learn_HubWorkflow1.png)  

3.向下滚动并从列表中选择 **Ruby’s Adventure: 2D Beginner** 项目。 

4.在项目对话框窗口中，选择 **下载项目(Download Project)**。

![download project](https://connect-cdn-prd-cn.unitychina.cn/20190829/learn/images/ff73b3ef-0da8-4ce6-90f4-b212c49b71c9_Download_project.png) 

5.下载完成后，选择 **打开项目(Open Project)**。

![open project](https://connect-cdn-prd-cn.unitychina.cn/20190829/learn/images/4b78560f-093e-4533-b84a-5c61cea9a122_Learn_HubWorkflow3_OpenProject.png) 

_* Unity Editor 将导入项目，并更新所有必要的软件包。_

6.在顶部菜单中，转到 **文件(File)** > **保存(Save)** 以保存您的 **Project** 版本。或者，您可以使用快捷键 **Ctrl + S**（Windows）或 **Cmd + S**（macOS）。

7.命名并保存场景(scene)。

## 3.导入资源（Assets） 
在您探索 **Unity Editor** 之前，让我们为本项目做一些准备。 
所有文件都在 **Unity Asset Store** 中，**资源** 创建者可以使用它来向其他 **Unity 用户** 提供工具或文件。 

- 要访问它，请打开编辑器，然后转到 **窗口(Window)** > **资源商店(Asset Store)**。 

下图为打开的资源商店 

![Assets store](https://connect-cdn-prd-cn.unitychina.cn/20190220/learn/images/ae23c8ab-90e5-4620-a02e-94980a81ab13_image.png) 

为了将本项目所需资源加载至场景中，您需要： 

1.在搜索栏中，输入 **2D Beginner: Tutorial**，然后单击搜索结果。 

2.在 **2D Beginner: Tutorial** 资源页上，单击 **下载(Download)**，然后等待下载完成。 

3.单击 **导入(Import)**。这将打开 **Unity Package** 窗口，其中列出了资源包含的所有文件。 

4.点击 **导入(Import)** 将这些文件导入项目。 

现在您已经完成所有的项目配置，接下来我们将探索 **Unity Editor** 是如何工作的！ 

## 4.Unity Editor 窗口 
让我们先浏览 **Unity Editor** 窗口。不用担心，您不需要记住每个细节！ 

本节仅使您大致了解每个窗口的功能，因此，当您更详细地探索编辑器时，您便知道要看屏幕的哪一部分。 

![Unity Editor windows](https://connect-cdn-prd-cn.unitychina.cn/20190829/learn/images/599c85d0-1f36-4119-83c8-4117c862271c_Hub_windows.png) 

### 项目窗口(Project window) 
**项目(Project)** 窗口列出了当前项目中的所有文件和目录。这些文件包括项目中使用的所有图像，声音和3D模型。它们统称为 **资源(Assets)**。 

![Project window](https://connect-cdn-prd-cn.unitychina.cn/20190902/learn/images/0b757093-1217-4863-a288-bf3c83b35889_ProjectWindowDemo.gif) 

- 打开 **演示文件夹(Demo folder)**，然后双击 **DemoScene**。这将打开一个 **场景(Scene)**，供您在本教程的其余部分中用作演示。

### 控制台窗口(Console window) 
![Console window](https://connect-cdn-prd-cn.unitychina.cn/20190902/learn/images/e0277327-5986-4406-ad26-275eb90637e3_Console_window.gif) 

让我们看一下 **控制台(Console window)** 窗口。默认情况下，**控制台窗口选项卡(Console window tab)** 位于 **项目窗口选项卡(Project window tab)** 旁边。

 **控制台(Console window)** 窗口将显示游戏产生的警告和错误，为您提供有关如何修复它们的有用信息。 

您可以通过拖放 **控制台选项卡(Console tab)** 以将其停靠在 **项目(Project)** 窗口旁边来移动它。 

 **控制台(Console window)** 窗口向您显示游戏正在产生的警告和错误，为您提供有关如何解决这些错误的有用信息。 

### 层级窗口(Hierarchy window)
在 **Unity** 中，您的游戏由 **场景** 组成。将场景视为游戏或其他环境中的关卡。在每个场景中，都有一个对象列表，该对象在该场景中具有位置。这些对象在 **Unity** 中称为 **GameObjects** 。 

您可以将 **GameObjects** 放置在父母和孩子的层次结构中。 **GameObjects** 可以是其他 **GameObjects** 的子级，允许您将它们分组移动（如果父级移动，则其所有子级都随之移动）。**层级窗口(Hierarchy window)** 显示场景中的所有 **GameObject** ，并显示父/子关系。 

![Hierarchy window](https://connect-cdn-prd-cn.unitychina.cn/20190902/learn/images/eb546045-7641-440f-ad82-a3843e652f4c_Hierarchy.gif) 

### 场景视图(Scene view) 
**场景视图(Scene view)** 是您当前加载的场景和 **层级(Hierarchy)** 中所有 **GameObjects** 的实时预览窗口。 

![Scene view](https://connect-cdn-prd-cn.unitychina.cn/20190205/learn/images/50206b5a-4057-49bc-8b89-159b020eb52b_image5.gif) 

### 游戏视图(Game view)
**游戏视图(Game view)** 是稍后在本教程中在编辑器中测试游戏时将显示的视图。

![Game view](https://connect-cdn-prd-cn.unitychina.cn/20190205/learn/images/736a4760-8995-4543-a72f-ff6ec973874d_image3.gif) 

默认情况下，**游戏视图(Game view)** 隐藏在 **场景视图(Scene view)** 选项卡的右侧。**场景视图(Scene view)** 允许您移动游戏对象并环顾整个场景，而 **游戏视图(Game view)** 显示了玩家在玩游戏时会看到的内容，这是摄像机看到的部分（图中的白色方框）。 

### 检查器窗口(Inspector window) 
_* 注：也可译为 观察窗口、属性窗口_ 

当您在 **层次(Hierarchy)** 或 **项目(Project)** 视图中选择一个项目时，**检查器(Inspector)** 将显示与该项目有关的所有数据。 

![Inspector](https://connect-cdn-prd-cn.unitychina.cn/20190205/learn/images/a262dc68-43d0-4fb6-8547-9a4b050cc08a_image3.gif) 

**GameObjects(游戏对象)** 

对于场景中的 **GameObjects(游戏对象)**，**Inspector(检查器)** 会显示有关该 **GameObjects** 的数据。Unity 使用 **Object - Component(对象-组件)** 模型，这意味着您的场景由添加了组件功能的 **GameObjects** 组成。例如，**Sprite Renderer(精灵渲染器)** 组件在场景中 **GameObject** 的位置显示图像，而 **Audio Source(音频资源)** 组件在 **Scene(场景)** 中 **GameObject** 的位置播放声音。所有 **GameObjects** 都从一个 **Transform(变换)** 组件开始，该组件允许您指定其在场景中的位置和旋转。所有其他组件都是可选的，您可以根据需要添加它们。 

**Assets(资源)** 

对于 **Assets(资源)**，**Inspector(检查器)** 显示 Unity 使用的**导入**设置。这些教程将重点介绍 **2D游戏** 中常见资源的导入设置并进行说明。 

![Assets in Inspector](https://connect-cdn-prd-cn.unitychina.cn/20190205/learn/images/ef0b0d4e-dd56-4e7c-aea9-1db719a70f22_image16.gif)

## 5.工具栏和导航UI 

#### Toolbar(工具栏) 
**Toolbar(工具栏)** 包含一系列有用的工具按钮，可帮助您设计和测试游戏。 

![Toolbar](https://connect-cdn-prd-cn.unitychina.cn/20190508/learn/images/26e31389-deec-408b-99eb-403f8b7cbb26_1.4_1_FullToolbar.png) 

##### Play buttons(Play 按钮)
![Play buttons](https://connect-cdn-prd-cn.unitychina.cn/20190508/learn/images/519674d4-2469-40b3-83e5-bb0108bad9c6_1.4_2_PlayButtons.png) 

- ##### Play(开始游戏)
    **Play** 用于在“层次结构”视图中测试当前加载的场景，以便您可以在编辑器中实时试用游戏。

- ##### Pause(暂停)
    您可能已经猜到了，**Pause** 可以让您暂停游戏视图中的游戏。它可以帮助您发现其他情况下不会出现的视觉问题或游戏玩法问题。 

- ##### Step(下一步 / 下一帧)
    **Step** 用于逐帧浏览暂停的场景。让您可以在游戏世界中实时寻找、查看变化，这是个非常有用的功能。 

##### Manipulating objects(操作对象) 

![Manipulating objects](https://connect-cdn-prd-cn.unitychina.cn/20190508/learn/images/e16ab2f0-9443-4f4a-bdb6-deb1817648a2_1.4_3_Toolbar.png) 

这些工具可在 **Scene(场景)** 视图中移动和操纵 **GameObject**。单击它们以使用。下表是每个工具所对应的快捷键： 

![quick key for manipulating objects](https://connect-cdn-prd-cn.unitychina.cn/20190829/learn/images/69f2d111-8418-469b-a54c-222d44c85b5f_toolbar_table.PNG) 

其它您也许想了解的快捷键： 

- F - 专注于选择的对象。如果忘记了 **GameObject** 在场景中的位置，只需在层次结构中选择它，然后按F使其在 **Scene(场景)** 视图中居中。 

#### Navigating with the mouse(用鼠标进行导航) 
在 **Scene(场景)** 视图中，可以使用： 
- 单击鼠标左键以在 **Scene** 中选中您的 **GameObject**。 
- 单击鼠标中键并拖动以使用手动工具移动 **Scene** 视图的摄像机。 
- 单击鼠标右键并拖动以使用 flythrough mode(飞越模式)——手动工具的一种，以此来旋转 **Scene** 视图摄像机。 

**注意：** 在3D项目中，您还可以通过单击鼠标右键并使用以下键旋转视图来移动相机： 

**左、右** 使用：**A** 和 **D** 

**前、后** 使用：**W** 和 **S** 

**上、下** 使用：**Q** 和 **E** 

有关在 **Scene(场景)** 视图中使用移动 **GameObjects** 的更多建议，请参阅：[Scene View Navigation](https://docs.unity3d.com/Manual/SceneViewNavigation.html)。 

## 6.布局(Layouts) 

### Default Layouts(默认布局) 
您可以为 **Unity 编辑器** 设置不同的布局。每种布局都有其自身的优势，您将了解哪种布局最适合您。让我们逐一查看，以了解可用的布局有哪些。 

要切换布局，请选择 **窗口(Window) > 布局(Layouts)**（或使用编辑器右上角的 **Layouts 下拉菜单**）。以下是布局描述： 

![layouts](https://connect-cdn-prd-cn.unitychina.cn/20190829/learn/images/04ec6800-3e8d-4d35-a205-21e89a78a207_Layout_keys.PNG) 

布局完全取决于个人喜好。**Ruby 2D RPG** 项目中的所有后续教程将使用 **Default** 布局，将 **Console(控制台)窗口** 停靠在Project窗口的一侧，就像在本教程的 **Console窗口** 部分中看到的那样。至少在本教程中，您应该从使用该布局开始。 

## 7.小结

现在，您对整个 **Unity 编辑器** 的组织方式有了更多的了解。如果在后续教程中提到 **Project(项目)窗口**，您应该知道在哪里可以找到它。本项目所需资源已添加到您的项目中，以方便您依照教程构建游戏。

_本章翻译完成，最后编辑时间 2019/11/30_

