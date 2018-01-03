# VSMediaPlayerExtension
Visual Studio Media Player Extension

The Visual Studio Media Player Extension is, at this time, an integrate Audio Player [yes, right now the 'Media' part of the name is mis-leading] but is something that we aim to change over the course of the development.

Based on the awesome BASS library by Ian Luck (http://un4seen.com), it can play all major audio files and online streams too (through PLS, M3U support).  Although there's an issue with the media scanner picking these files up at the moment!

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

If you have not already downloaded the media player
