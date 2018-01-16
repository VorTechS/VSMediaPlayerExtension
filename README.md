# Visual Studio Media Player Extension

The Visual Studio Media Player Extension is, at this time, an integrate Audio Player [yes, right now the 'Media' part of the name is mis-leading] but is something that we aim to change over the course of the development.

Based on the awesome BASS library by Ian Luck (http://un4seen.com), it can play all major audio files and online streams too.

Visualization support is provided through the BASSVIS plugin, and in this version is limited to the WinAMP AVS Studio.  The 'best' AVS Studio modules are included which support Windows 7 and above without crashing.  (It's taken many years to find the ones that cause AVS to crash on later version of Windows!).  The eagle eyed amongst you will notice that 'Toumas: AVS Gone Bad' has been removed due to the explicit nature of the text content.

Supported Visual Studio Targets
===============================

The base manifest includes the following targets for installation:

        <InstallationTarget Version="[14.0,16.0)" Id="Microsoft.VisualStudio.Pro" />
        <InstallationTarget Version="[14.0,16.0)" Id="Microsoft.VisualStudio.Enterprise" />
        <InstallationTarget Version="[14.0,16.0)" Id="Microsoft.VisualStudio.Community" />

...meaning that all 'standard' Visual Studio 2015 and 2017 editions are supported.

Installation
============

If you have not already downloaded the media player, you can do so through the Visual Studio Market Place (https://marketplace.visualstudio.com/items?itemName=VorTechS.VisualStudioMediaPlayer), and follow the normal installation process.

If you have been provided with the .VSIX file, simply double click on the file to launch the VSIX Installer, and choose the editions of Visual Studio you would like to make the extension available to.

Configuration
=============

Configuration of the extension is performed using the Visual Studio menu 'Tools' and 'Options' dialog.  You will see a 'Visual Studio Media Player' category.  The default options are great for getting started with, but you must add at least one 'Media Path' before the plugin will successfully activate.

Advanced Visualization
======================

The WinAMP AVS Editor will NOT retain any configuration settings you make unless you are able to create a folder called 'Plugins' inside your Visual Studio IDE directory.  Typically this will reside in:

        C:\Program Files (x86)\Microsoft Visual Studio <Version> 

in the sub-folder: 

        <Edition>\Common7\IDE

For example:

        C:\Program Files (x86)\Microsoft Visual Studio\2017\Enterprise\Common7\IDE

should have the path:

        C:\Program Files (x86)\Microsoft Visual Studio\2017\Enterprise\Common7\IDE\Plugins
        
