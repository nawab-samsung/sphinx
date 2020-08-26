# Install Tizen Studio

This page walks you through default installation of Tizen Studio. Follow the steps or video demo for getting hands on with TV app development, and get yourself up and running instantly.

<style>


.center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 100%;
}
.tabs {
  display: block;
  display: flex;
  -webkit-flex-wrap: wrap;
  -moz-flex-wrap: wrap;
  flex-wrap: wrap;
  margin: 0;
  overflow: hidden; }
  .tabs [class^="tab"] label,
  .tabs [class*=" tab"] label {
    cursor: pointer;
    display: block;
    font-size: 1.1em;
    font-weight: 300;
    line-height: 1em;
    padding: 1rem 0;
    text-align: center; }
  .tabs [class^="tab"] [type="radio"],
  .tabs [class*=" tab"] [type="radio"] {
    border-bottom: 1px solid #008aee;
    cursor: pointer;
    -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
    display: block;
    width: 100%;
    -webkit-transition: all 0.3s ease-in-out;
    -moz-transition: all 0.3s ease-in-out;
    -o-transition: all 0.3s ease-in-out;
    transition: all 0.3s ease-in-out; }
    .tabs [class^="tab"] [type="radio"]:hover, .tabs [class^="tab"] [type="radio"]:focus,
    .tabs [class*=" tab"] [type="radio"]:hover,
    .tabs [class*=" tab"] [type="radio"]:focus {
      border-bottom: 5px solid #008aee; }
    .tabs [class^="tab"] [type="radio"]:checked,
    .tabs [class*=" tab"] [type="radio"]:checked {
      border-bottom: 10px solid #008aee; }
    .tabs [class^="tab"] [type="radio"]:checked + div,
    .tabs [class*=" tab"] [type="radio"]:checked + div {
      display:block }
    .tabs [class^="tab"] [type="radio"] + div,
    .tabs [class*=" tab"] [type="radio"] + div {
      padding: rem 0;
      width: inherit;
      display: none;
      margin-inline-start: 800%;
      -webkit-transition: all 0.3s ease-in-out;
      -moz-transition: all 0.3s ease-in-out;
      -o-transition: all 0.3s ease-in-out;
      transition: all 0.3s ease-in-out; }
  .tabs .tab-2 {
    width: 33% }
    .tabs .tab-2 [type="radio"] + div {
      width: 300%;
      margin-left: 0; }
    .tabs .tab-2 [type="radio"]:checked + div {
      margin-left: 0%; }
    .tabs .tab-2:last-child [type="radio"] + div {
      margin-left: 0%; }
    .tabs .tab-2:last-child [type="radio"]:checked + div {
      margin-left: -200% ; }
.tabs .tab-3 {
    width: 33%; }
    .tabs .tab-3 [type="radio"] + div {
      width: 300%;
      margin-left: 0; }
    .tabs .tab-3 [type="radio"]:checked + div {
      margin-left: 0%; }
    .tabs .tab-3:last-child [type="radio"] + div {
      margin-left: 0%; }
    .tabs .tab-3:last-child [type="radio"]:checked + div {
      margin-left: -200%; }
.tabs .tab-4 {
    width: 33%; }
    .tabs .tab-4 [type="radio"] + div {
      width: 300%;
      margin-left: -100%; }
    .tabs .tab- [type="radio"]:checked + div {
      margin-left: 0%; }
    .tabs .tab-4:last-child [type="radio"] + div {
      margin-left: 0%; }
    .tabs .tab-:last-child [type="radio"]:checked + div {
      margin-left: -200%; }
video {
  width: 100%;
  height: auto;
}
</style>

<div class="tabs">
 
  <div class="tab-2">
    <label for="tab2-1"><b>Windows&reg;</b></label>
    <input id="tab2-1" name="tabs-two" type="radio" checked="checked">
  <div>  
  
# Install Tizen Studio on Windows&reg;

This page explains the process to download and install Tizen Studio on your development hardware.

To have optimal installation experience, follow these steps chronologically:

- System prerequisites
  - Hardware requirements
  - Software requirements
- Launch installer
- Verify installation

## System Prerequisites

Ensure that the following system prerequisites are met:

### Hardware Requirements
<table>
  <tr>
      <td width=150px>CPU</td>
    <td colspan="3" width=50px>Dual Core, 2Ghz or faster</td>
  </tr>
  <tr>
    <td>Architecture</td>
    <td width=520px>x32 or x64 </td>
  </tr>
  <tr>
    <td>Memory</td>
    <td colspan="3">3GB or more </td>
  </tr>
  <tr>
    <td>Disk space</td>
    <td colspan="3">6 GB or more </td>
  </tr>
</table> 

### Software Requirements
<table>
  <tr>
    <th colspan="2" align=left>Windows</th>
  </tr>
  <tr>
    <td width=150px>Version</td>
    <td width=520px>7/8/10</td>
  </tr>
  <tr>
    <td>Bit</td>
    <td>32 or 64 bit</td>
  </tr>
  <tr>
    <td>Tizen Studio setup file</td>
    <td><a href="https://developer.tizen.org/development/tizen-studio/download#">Download</a></td>
  </tr>
</table>

## Launch Installer
 
To launch the installer, follow these steps:

1. Double click **web-ide_Tizen_Studio_x.x_windows-64.exe** file.
	> [!NOTE] 
	>**x.x** represents the latest version of Tizen Studio, for example:web-ide_Tizen_Studio_**3.7**_windows-64.exe.

2. Accept the software license.
   
   > [!NOTE]
   > The license contains important legal notices for using Tizen Studio. Read it fully, and click **Accept** only if you agree with the license statement.

   ![Tizen Studio License Agreement](./media/install_sdk_license.png)

3. Click **Browse** and specify a new directory to set the SDK data location. 

   ![Set SDK and data location](./media/install_sdk_directory.png)
  
   >[!NOTE] 
   >If the new directory is valid, it shows no errors.

4. Click **Install**.
5. Click **Finish** to close the installer.

   ![Installation complete](./media/migration_finish_instal.png)

   >[!NOTE]
   > - If you install Tizen Studio in a directory that requires administrator privileges for access, such as `C:\Program Files`, then administrator privileges are required to run the Tizen SDK tools.
   > - If you want to install additional platforms and tools, launch Package Manager by selecting the Launch the Package Manager **check box** and click **Finish**.
   > - Use Tizen Package Manager, to install and update additional tools. 
   > - For more information on the Package Manager, see [Updating Tizen Studio](./update-sdk.md).

    ### Quick Hands-on Installation Demo
   
   ![Installation complete](./media/installw.gif)

# Verify Installation   

   To verify whether the installation is successful or not, click **Tizen Studio icon**. Tizen Studio startup window must appear.
  </div>
</div>

<div class="tab-4">
  <label for="tab4-4"><b>Ubuntu&reg;</b></label>
    <input id="tab4-4" name="tabs-two" type="radio">
<div>  

# Install Tizen Studio on Ubuntu&reg;

This page guides you with downloading and installing Tizen Studio on your development hardware. 

To have the optimal installation experience, follow these steps chronologically:

- System prerequisites
  - Hardware requirements
  - Software requirements
- Install dependencies
- Launch installer
- Verify installation

<style type="text/css">
a.clickable   { width: 100%; height: 100%; }
a.clickable:hover   { background-color:; color: #FFFFF; }
</style>
### System Prerequisites

Ensure that the following system prerequisites are met:

#### Hardware Requirements
<table>
  <tr>
      <td width=150px>CPU</td>
    <td colspan="3" width=50px>Dual Core, 2Ghz or faster</td>
  </tr>
  <tr>
    <td>Architecture</td>
    <td width=520px>x32 or x64 </td>
  </tr>
  <tr>
    <td>Memory</td>
    <td colspan="3">3GB or more </td>
  </tr>
  <tr>
    <td>Disk Space</td>
    <td colspan="3">6 GB or more </td>
  </tr>
</table> 

#### Software Requirements
<table>
  <tr>
    <th colspan="2" align=left>Ubuntu</th>
  </tr>
  <tr>
    <td width=190x>Version</td>
    <td width=520px>16.04/ 14.04/ 18.04</td>
  </tr>
  <tr>
    <td>Bit</td>
    <td>32 or 64 bit</td>
  </tr>

  <td>Tizen Studio setup file</td>
    <td>
    <a href="https://developer.tizen.org/development/tizen-studio/download#" class="clickable" target="_blank">Download</a></td>
  </tr>
</table>

	
## Install Dependencies

The installer package consists of basic and immediate libraries. However, Tizen Studio application requires additional libraries in order to work flawlessly. 

To install the dependencies, open the terminal and execute the following commands: 

`
sudo apt install expect; sudo apt install gtk2-engines-pixbuf;  sudo apt install libgnome2-0; sudo apt install qemu-user-static;
sudo apt install libwebkitgtk-1.0-0; sudo apt install libwebkitgtk-1.0-0 cpio rpm2cpio; sudo apt install gettext; sudo apt install gksudo; sudo apt install module-init-tools; sudo apt install libudev-dev; sudo apt install libsdl1.2debian; sudo apt install bridge-utils; sudo apt install openvpn;
 `

 ### Install Emulator Dependencies

The Emulator also requires a few additional libraries to work smoothly. To install these dependencies, open the terminal and enter the following command:

  ` sudo apt install acl bridge-utils openvpn libfontconfig1 libglib2.0-0 libjpeg-turbo8 libpixman-1-0 libpng12-0 libsdl1.2debian libsm6 libv4l-0 libx11-xcb1 libxcb-icccm4 libxcb-image0 libxcb-randr0 libxcb-render-util0 libxcb-shape0 libxcb-xfixes0 libxi6`

## Launch Installer 

Navigate to the directory where you have saved the installer file and proceed with the further instructions. 

To launch the installer, follow these steps:

1. Open the terminal and execute the following commands:
	
	- `chmod +x web-ide_Tizen_Studio_x.x_ubuntu-64.bin`
	- `./web-ide_Tizen_Studio_x.x_ubuntu-64.bin` 
	>Note:
	>
	>**x.x** represents the latest version of Tizen Studio, for example: web-ide_Tizen_Studio_**3.7**_ubuntu-64.bin.
2. Accept the software license.
   
   > [!NOTE]
   >The license contains important legal notices for using Tizen Studio. Read it fully, and click **Accept** only if you agree with the license terms.

   ![Tizen Studio License Agreement](./media/install_sdk_license.png)

3. Click **Browse** and specify a new directory to set the SDK location and the SDK data location.

   ![Set SDK and data location](./media/install_sdk_directory.png)
   
   > [!NOTE]
   >If the new directory is valid, it shows no errors.
4. Click **Install**.
5. Click **Finish** to close the installer.

   ![Installation complete](./media/migration_finish_instal.png)

   > [!NOTE]
   >If you want to install additional platforms and tools, launch Package Manager by selecting the Launch Package Manager **check box** and click **Finish**.
   > - Use Tizen Studio Package Manager, to install and update additional tools. 
   > - For more information on the Package Manager, see [Updating Tizen Studio](./update-sdk.md).

### Verify Installation
   
To verify whether the installation is successful or not, click **Tizen Studio icon**. Tizen Studio startup window must appear.

  </div>
</div>

<div class="tab-3">
  <label for="tab3-3"><b>macOS&reg;</b></label>
    <input id="tab3-3" name="tabs-two" type="radio">
      <div>


# Install Tizen Studio on macOS&reg;

This page explains the process to download and install Tizen Studio on your development hardware. 

To have the optimal installation experience, follow these steps chronologically:

- System prerequisites
   - Hardware requirements
   - Software requirements
   - Additional requirements
- Launch installer
- Verify installation

<style type="text/css">
a.clickable   { width: 100%; height: 100%; }
a.clickable:hover   { background-color:; color: #FFFFF; }
</style>

## System Prerequisites

Ensure that the following system prerequisites are met:

### Hardware Requirements
<table>
  <tr>
      <td width=150px>CPU</td>
    <td colspan="3" width=50px>Dual Core, 2Ghz or faster</td>
  </tr>
  <tr>
    <td>Architecture</td>
    <td width=520px>x64 only</td>
  </tr>
  <tr>
    <td>Memory</td>
    <td colspan="3">3GB or more </td>
  </tr>
  <tr>
    <td>Disk Space</td>
    <td colspan="3">6 GB or more </td>
  </tr>
</table> 

### Software Requirements
<table>
  <tr>
    <th colspan="2" align=left>MacOSX</th>
  </tr>
  <tr>
    <td width=190px>Version</td>
    <td width=520px>10.13 (High Sierra)<br>10.12 (Sierra)<br>10.11 (El Captain)</td>
  </tr>
  <tr>
    <td>Bit</td>
    <td>64 bit only</td>
  </tr>

  <tr>
    <td>Tizen Studio setup file</td>
    <td><a href="https://developer.tizen.org/development/tizen-studio/download#" class="clickable" target="_blank">Download </a></td>
  </tr>
</table>


### Additional Requirements

<table>
<thead>
<tr>
<th>Component</th>
<th>Requirement</th>
</tr>
</thead>
<tbody>
<tr>
<td>Prerequisite packages (<code>msgfmt</code>) to build PO files
</td>
<td>On the terminal prompt, type the following commands:
<pre><code>$ brew install gettext
$ brew link gettext -force
$ which msgfmt
/usr/local/bin/msgfmt
</code></pre>
<strong>Note</strong><br>
To install Homebrew, see the<a href="http://brew.sh/">Homebrew documentation</a>.
</td>
</tr>
</tbody>
</table>


## Launch Installer
 
To launch the installer, follow these steps:

1. Double click on the downloaded installer file **web-ide_Tizen_Studio_x.x-64.dmg**.
   
   > [!NOTE]
   >**x.x** represents the latest version of Tizen Studio, for example:web-ide_Tizen_Studio_**3.7**-64.dmg.

2. Accept the software license.
   
   > [!NOTE]
   > The license contains important legal notices for using Tizen Studio. Read it fully, and click **Accept** only if you agree with the license terms.

   ![Tizen Studio License Agreement](./media/install_sdk_license.png)
3. Click **Browse** and specify a new directory to set the SDK location and the data location. 
   
   ![Set SDK and data location](./media/install_sdk_directory.png)
   
   > [!NOTE]
   > If the new directory is valid, it shows no errors.
4. Click **Install**.
5. Click **Finish** and close the installer.
   
   ![Installation complete](./media/migration_finish_instal.png)
   
   > [!NOTE]
   > - If you want to install additional platforms and tools, launch  Package Manager by selecting the Launch Package Manager **check box** and click **Finish**.
   > - Use Tizen Studio Package Manager, to install and update additional tools. 
   > - For more information on the Package Manager, see [Updating Tizen Studio](./update-sdk.md).

## Verify Installation

To verify whether the installation is successful or not, click **Tizen Studio icon**. Tizen Studio startup window must appear.



</div>

      