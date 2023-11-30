# PowerShell Pre-Workout

My boosted and caffeinated mix of tools to help jump start your PowerShell session!

<img src="images/banners/_a57f5485-9e3f-4e3f-9a11-2be1b1ea4179.jpg" alt="An image generated by Bing Image Creator. Prompt: hooded robot hacker wearing a PowerShell shirt, drinking a powerful energy drink with energy swirling around the cup, surrounded by swirling energy, floating in the air, cinematic, hacker professional photography, studio lighting, studio background, advertising photography, intricate details, hyper-detailed, ultra realistic, 8K UHD, PowerShell" width="400" />

## Contents

- [New-ProfileWorkspace](#newprofileworkspace)
- [New-DotSourcedProfile](#newdotsourcedprofile)
- [Install-PowerShellISE](#installpowershellise)
- [Get-MsModules](#getmsmodules)
- [Install-MsModules](#installmsmodules)
- [Update-MsModules](#updatemsmodules)
- [Get-RecommendedModules](#getrecommendedmodules)
- [Install-RecommendedModules](#installrecommendedmodules)

<a name="newprofileworkspace"></a><div id='newprofileworkspace' />
## New-ProfileWorkspace

### Synopsis

Setup a folder and VS Code Workspace for maintaining your PowerShell profiles, VS Code settings, and Windows Terminal settings.

### Description

I wanted an easy way to maintain all of my CurrentUser PowerShell profiles, and my settings files for Visual Studio Code and Windows Terminal. There are probably easier ways to accomplish this, but my basic goal was to not have to hunt for these files across the file system in order to edit them. This over-engineered idea creates a folder that contains:

- Junction points to the locations of your CurrentUser PowerShell and Windows PowerShell folders
- Junction points to the locations of your settings for VS Code and Windows Terminal
- Structural artifacts in case you want to save this as a repository
  - A Visual Studio Code workspace file that opens this new folder
  - EditorConfig and Visual Studio Code settings files for consistent editing
  - A .gitignore file in case you want to use this as a git repository (test?)

Script: [New-ProfileWorkspace.ps1](New-ProfileWorkspace.ps1)
Status: Working :runner:


<a name="newdotsourcedprofile"></a><div id='newdotsourcedprofile' />
## New-DotSourcedProfile

I need to automate this one still, but it will be a script that creates one central profile script and then sets each CurrentUser profile to dot source that central profile for easier sync across all of your profiles for PowerShell, PowerShell ISE, Visual Studio Code, Windows PowerShell, etc.

<a name="installpowershellise"></a><div id='installpowershellise' />
## Install-PowerShellISE

Install the PowerShell ISE if it was removed. It can be helpful to keep the ISE installed for compatibility testing.

Script: [Install-PowerShellISE.ps1](Install-PowerShellISE.ps1)
Status: Working :runner:

<a name="getmsmodules"></a><div id='getmsmodules' />
## Get-MsModules

List all of the Microsoft PowerShell modules that you need for working with Azure, Microsoft 365, or Microsoft Graph.

Script: [Get-MsModules.ps1](Get-MsModules.ps1)
Status: In Progress :construction_worker:

<a name="installmsmodules"></a><div id='installmsmodules' />
## Install-MsModules

Quickly install all or any of the Microsoft PowerShell modules that you need for working with Azure, Microsoft 365, or Microsoft Graph.

<a name="updatemsmodules"></a><div id='updatemsmodules' />
## Update-MsModules

Quickly update all or any of the Microsoft PowerShell modules that you need for working with Azure, Microsoft 365, or Microsoft Graph.

<a name="getrecommendedmodules"></a><div id='getrecommendedmodules' />
## Get-RecommendedModules

Get a list of recommended PowerShell modules authored by  Microsoft and the community.

<a name="installrecommendedmodules"></a><div id='installrecommendedmodules' />
## Install-RecommendedModules

Install your choice of recommended PowerShell modules authored by  Microsoft and the community.
