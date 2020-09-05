# Template settings for Remote Develop extention on VSCode

## How to use

1. Install required tools.
   - VisualStudioCode
   - Git
   - Docker
1. Create your repository from this template repository.
2. Clone your repository to local.
3. Open local folder with VSCode.
4. Install [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack) extention.
5. Modify docker-compose.yml and devcontainer.json
6. Press F1 key to run `Remote-Containers:Open Folder in Container` and chose your folder.

## Files

- `docker-compose.yml`  
  Base settings of docker containers for development.
  When you run `docker-compose up`, only this file is used as docker settings but bellow files are not used.
- `.devcontainer/docker-compose.yml`  
  Extra docker settings. When you run containers with VSCode extention, this settings is applied additionally.
- `.devcontainer/devcontainer.json`  
  Settings of VSCode extention `Remote Development`. 
  - `dockerComposeFile` : Specify `docker-compose.yml` files to apply.
  - `settgings` : Set specific VSCode settings for remote environment.
  - `extentions` : Set pre-installed extentions for remote environment.


