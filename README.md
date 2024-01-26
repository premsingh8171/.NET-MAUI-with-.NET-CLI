# .NET MAUI with .NET CLI (Command Line Interface)
This article describes how to develop a .NET MAUI app with the .NET CLI (Command Line Interface).

.NET Multi-platform App UI (.NET MAUI) is a cross-platform framework for creating native mobile and desktop apps with C# and XAML that can run on Android, iOS, macOS, and Windows from a single shared code-base.

<h2> 1. Install .NET SDK.</h2>
https://dotnet.microsoft.com/en-us/download

<h2>2. Install .NET MAUI workload with the dotnet CLI. A .NET "workload" is a collection of packs. Launch a command prompt and enter the following:</h2>
<code style="color" : blue">dotnet workload install maui</code>
<br>
<br>
Check that the MAUI workload installs successfully.<br><br>
<code style="color" : blue">dotnet workload list</code>


<h2>3. Verify and install missing components with maui-check command line utility.</h2><br>
<code style="color" : blue">dotnet tool install -g redth.net.MAUI.check</code><br><br>
<code style="color" : blue">maui-check</code>


<h2>4. Create a new folder and a new MAUI app.</h2><br>
<code style="color" : blue">mkdir MyMauiApp</code><br><br>
<code style="color" : blue">cd MyMauiApp</code><br><br>
<code style="color" : blue">dotnet new maui</code><br>


<h2><p></p>5. The "dotnet new maui" command generates a template for a .NET MAUI app with all the necessary project, C#, and XAML files. You can use any editor such as Notepad or Visual Studio Code to edit the files.

If you are using Visual Studio Code, enter the following command in the Command Prompt to view the source code generated in the "MauiQRCodeApp" folder.</p></h2><br>

code .

<h2>6. Start an Android Emulator with the following command:</h2>

   
        "C:\Program Files (x86)\Android\android-sdk\emulator\emulator.EXE" -no-boot-anim -avd pixel_5_-_api_30 -prop monodroid.avdname=pixel_5_-_api_30
                
<h2>7. Run the MAUI app in an Android Simulator.</h2>

dotnet build -t:Run -f net6.0-android




<img src="https://mauiman.dev/images/maui_android.png" height="1080" widrth="720"/>
   
