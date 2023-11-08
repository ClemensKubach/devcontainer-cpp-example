# Devcontainer C++ example

## Getting started
1. Install and **start** vscode, Docker-Desktop and (optionally) git.
2. Download and use [this repository](https://github.com/ClemensKubach/devcontainer-cpp-example) from as template to create your own. To do this, you have 3 option.
- Create an own GitHub repository via template
- Download template as zip file.
- Clone the repository and copy the resulting files into your own repository. (Do not commit any changes to the original repository!)
3. Open the folder of your local repository on your machine in vscode.
4. In vscode on the left side click on the extensions-icon. Search for the following extensions and install them: `Docker`, `Dev Containers`. 
5. Press Command/Control + Shift + P and search for `Dev Container`. Select something like `Dev Container: (Re)build Container`. The first time, this can take a while (~1h) because a docker image, some tools and the required dependencies are downloaded and built with a single core (multi-core build results in errors).

**Your local setup is done, now you are working in your dev container.**

Last steps for cpp development:
1. Asjust the `"cmake.sourceDirectory": "/workspaces/<repo-name>/<optional-sub-folder>"` field in `.vscode/settings.json` to your own source directory.
2. Build/compile using the bottom menu of vscode

## Further Information
The next steps are independent of your local machine and the most stuff has already been setup.
Just follow the last steps:
- At the bottom left corner you can validate that you are now using a remote connection to your local dev container: `c++ at dektop-linux`.
- Via clicking on the blue corner, you can "Close the remote connection" and "Reopen in Container".
- For syncing your changes with others, you use git. You can use it via terminal and via GUI (the Source Control-icon on the left side in vscode). I recommend the use of the GUI. Ask for explaination. In general, the most important commands are pull/fetch, add, commit and push.

Via the bottom menu of vscode, you can build and run your files.

**To access the desktop/gui of your devcontainer:**
Open http://localhost:6080/ in a browser.
