
# MAmods
Simple visual modding for Midair through hooking DX11.

### Method of operation
DLL injection to hook `IDXGISwapChain::Present`, `ID3D11DeviceContext::DrawIndexed` and `ID3D11DeviceContext::PSSetShaderResources`.

### Minimal requirements
 - Windows 10
 - [Windows 10 SDK](https://developer.microsoft.com/en-us/windows/downloads/windows-10-sdk/)
 <!--- - Access to a DLL injector -->

The binary is compiled for Windows SDK version 10.0.17763.0 with platform toolset v142 (2019).

So the minimal requirements are Windows 10 with MSVC++ versions 2019 and above.

### Features
- Hide in game crosshair
- Load up to 20 custom crosshairs
- Custom crosshair for each weapon

### Getting started
 1. Download and extract the [latest release]() from the [Release](/Release) folder which contains everything you need to run the mod.
 2. Run Midair.
 3. Alt+Tab out of Midair and then run **midair.bat** from the extracted release file. A console window should appear for Midair with some basic print out. 
![Image](https://cdn.discordapp.com/attachments/596698457532792833/758148212657225758/successful_inject.png)
 4. Enter back into Midair and press the **INSERT key** to toggle the mod menu. You can now interact with the menu using your mourse to turn features on or off.
![Image](https://cdn.discordapp.com/attachments/596698457532792833/758148089789284372/unknown.png)

### How to use custom crosshairs
 1. Find your local installation of Midair (`Right click on Midair in Steam` > `Manage` > ` Browse local files`).
 2. Navigate to `%YOUR LOCAL INSTALL OF MIDIAR% \MidairCE\Binaries\Win64` which should contain a file called **MidairCE-Win64-Test.exe**. 
 3. Put all crosshairs in this folder. All crosshair images **must be .png** and follow the naming convention of **crosshairX.png**. So the crosshair files can be named `crosshair0.png` to `crosshair19.png`.

### Custom crosshair pack
A pack of custom crosshairs is provided [here](/Files/Crosshairs.rar).