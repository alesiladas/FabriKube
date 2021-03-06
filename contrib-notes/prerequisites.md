# Installing Development Pre-requisites

The essential tools you will need are *npm*, *docker*, *docker-compose* and a code editor, for example *Atom* or *VSCode*. Samples are held in GitHub so *git* will be needed as well.

Automatic installations scripts are available for [Ubuntu](./prerequisites-ubuntu.md)

The recommended *minimum* versions are:
- *Docker*: v17.03
- *Kubectl*: client: v1.10.1, server: v1.10.0
- *npm*: v5.5.1
- *node.js*: v8.9.1

## Manual Installation

### 1. Installing NVM
We highly recommend installing NVM to easily install and manage versions of [node.js](https://nodejs.org/en/) and [npm](https://www.npmjs.com/). The main runtime uses node.js and npm is used for package management and dependency installation. The runtime requires a version equal to or higher than v8.9.1, but not Node v9 which isn't supported.

[Official nvm GitHub repository](https://github.com/creationix/nvm)

### 2. Kernel Packages
If running on Ubuntu Trusty, it is necessary to obtain additional Kernel packages to enable use of the [AUFS storage driver](https://docs.docker.com/engine/userguide/storagedriver/aufs-driver/#renaming-directories-with-the-aufs-storage-driver) for Docker.

### 3. Installing Docker Engine
The Docker Engine is essential for running system tests and running the HyperLedger Fabric.

[Official Docker Engine Installation Guide](https://docs.docker.com/engine/installation/)

### 4. Installing Kubectl
[Kubectl](https://kubernetes.io/docs/reference/kubectl/overview/) is used for easily configuring and starting HyperLedger Fabric.

[Official Kubectl Installation guide](https://kubernetes.io/docs/tasks/tools/install-kubectl/)

### 5. Installing Git
This is probably already installed on most Linux machines. Pay particular attention to [setting up the SSL keys](https://help.github.com/enterprise/2.7/user/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/#platform-linux) that are required.

[Official Git Download](https://git-scm.com/downloads)

## Optional Installs

### 1. Installing an editor

{{site.data.conrefs.composer_full}} allows you to edit its project files with any editor. We recommend using either Atom or Visual Studio Code, as not only do both have excellent support for Javascript development, a `.cto` file syntax highlighting plugin exists for these editors.

**Atom**

[Atom](https://atom.io/) is a very popular editor and several contributors use it.

[Official Atom installation guide](http://flight-manual.atom.io/getting-started/sections/installing-atom/)

Suggested Plugins:

* [Composer Atom Syntax Highlighter](https://github.com/hyperledger/composer-atom-plugin) A plugin for model file highlighting.

* [File Icons](https://atom.io/packages/file-icons) is a useful UI enhancement to show different icons for different files.


**Visual Studio Code**

[Visual Studio Code](https://code.visualstudio.com/) is a lightweight and powerful editor.

Extensions may be installed into VS Code by searching the Extensions repository for the desired extension package and selecting the install option once identified. Suggested extentions include:

* Composer VS Code Plugin. Provides syntax highlighting for CTO files within VS Code

* ESLint. Integrates ESLint into VS Code.

* TSLint. Integrates the tslint linter for the TypeScript language into VS Code.

* EditorConfig for VS Code. Enables the definition and maintainance of consistent coding styles between different editors and IDEs.

## License <a name="license"></a>
Hyperledger Project source code files are made available under the Apache License, Version 2.0 (Apache-2.0), located in the LICENSE file. Hyperledger Project documentation files are made available under the Creative Commons Attribution 4.0 International License (CC-BY-4.0), available at http://creativecommons.org/licenses/by/4.0/.