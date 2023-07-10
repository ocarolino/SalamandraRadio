# How to install Salamandra

- [Downloading Salamandra](#downloading-salamandra)
- [Installable version](#installable-version)
  - [Migrating from Portable Version](#migrating-from-portable-version)
    - [Versions before 0.5.3](#versions-before-053)
    - [Versions from 0.5.3 onwards](#versions-from-053-onwards)
- [Portable Version](#portable-version)
  - [Installing Salamandra](#installing-salamandra)
  - [Updating Salamandra](#updating-salamandra)
    - [From 0.5.3 onwards](#from-053-onwards)
    - [Versions before 0.5.3](#versions-before-053)

## Downloading Salamandra

To download Salamandra, you just need to go to the [project's main page](https://github.com/ocarolino/SalamandraRadio) and look for the **Releases** section.

<p align="center">
<img src="Images/How To Install/SalamandraGitHub.png" alt="Página do Salamandra no GitHub" />
</p>

Then click **on the version being displayed** and you will open at the page with the download link for Salamandra.

<p align="center">
<img src="Images/How To Install/SalamandraReleases.png" alt="Página de Releases do Salamandra" />
</p>

On this page you will always see the latest version of Salamandra at the top, with a brief description of the new features or bug fixes it contains.

Look for the link **Salamandra.rar** (for the portable version) or **Salamandra-installer.rar** (for the installable version), and then click on the desired version to download the program.

## Installable version

Download the **Salamandra-installer.rar** file, then extract it and run **Salamandra-installer.exe**. After doing that, just follow the installer step by step.

<p align="center">
<img src="Images/How To Install/ExtractingSalamandraInstaller.webp" alt="Extração do Instalador do Salamandra" />
</p>

To update, just follow the same process of downloading and running the installer and the whole process will be done automatically.

### Migrating from Portable Version

If you are using the portable version and want to migrate to the installable version, the process is also quite simple, but you will need to be careful. Follow the steps below, checking which version you currently have installed.

#### Versions before 0.5.3

If you are on a version prior to 0.5.3 and want to upgrade, you can just install Salamandra in the same folder that the portable version is already installed. But if you don't want to do that, follow the steps below:

1. Install Salamandra and **open it for the first time**, so that it prepares the configuration folders.
2. Access the folder **%appdata%/NovaBR Softwares/Salamandra** and delete the files contained therein. **THIS STEP IS VITAL FOR YOUR SETTINGS TO BE CORRECT.**
3. Copy the **application_settings.json** and **directory_library.json** files from the portable version folder to the **%appdata%/NovaBR Softwares/Salamandra** folder.

<p align="center">
<img src="Images/How To Install/MigratingSalamandraSettings.webp" alt="Como migrar as configurações portáteis para a instalação" />
</p>

#### Versions from 0.5.3 onwards

1. Install Salamandra and **open it for the first time**, so that it prepares the configuration folders.
2. Access the folder **%appdata%/NovaBR Softwares/Salamandra** and delete the files contained therein. **THIS STEP IS VITAL FOR YOUR SETTINGS TO BE CORRECT.**
3. Access the Settings directory of the portable version folder and copy all its contents to the **%appdata%/NovaBR Softwares/Salamandra** folder.

<p align="center">
<img src="Images/How To Install/MigratingSalamandraFromSettingsFolder.webp" alt="Como migrar as configurações portáteis da versão nova para a instalação" />
</p>

## Portable Version

### Installing Salamandra

For the portable version of Salamandra an installation process is not necessary, you just download the file **Salamandra.rar** in a folder that is convenient for you and then extract it and look for **Salamandra.exe** to run it.

<p align="center">
<img src="Images/How To Install/ExtractingSalamandra.webp" alt="Extração do Salamandra" />
</p>

After extraction you can create a shortcut on your desktop to open Salamandra more quickly in the future. Just right-click on the executable and go to the **Send to > Desktop** option.

### Updating Salamandra

#### From 0.5.3 onwards

If you are on version 0.5.3 and want to upgrade to a newer version, follow the procedure below.

You must access the Salamandra folder and delete all files and folders, **EXCEPT** the **Settings** folder. In this folder are all the information for Salamandra's settings.

<p align="center">
<img src="Images/How To Install/UpdatingSalamandraSettingsFolder.webp" alt="Atualização do Salamandra" />
</p>

After that, just repeat the process to download a more current version and extract it in the same folder. By keeping this folder, you will have all the settings preserved, so you can enjoy the new features without interfering with what you were already configuring.

#### Versions before 0.5.3

If you are on version 0.5.2 or below and want to upgrade to 0.5.3 or above, follow the procedure below.

The upgrade process to the portable version is simple, but you need to be careful. Just open the folder where you extracted it and delete all the files, **EXCEPT** **application_settings.json** and **directory_library.json**, because these are the files where Salamandra keeps its settings.

<p align="center">
<img src="Images/How To Install/UpdatingSalamandra.webp" alt="Atualização do Salamandra" />
</p>

After that, just repeat the process to download a more current version and extract it in the same folder. By keeping both files, you will have all the configurations preserved, so you can enjoy the new features without interfering with what you were already configuring.