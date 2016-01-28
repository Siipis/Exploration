# Exploration
This is a learning project for NW/Node-Webkit

## What you need to join
### Source Control
Start by downloading Git [here](https://git-scm.com/downloads). What you want is the Git Bash console that replaces the default console (like cmd.exe). 

Downloading Git alone already allows you to download the source files. It is however recommended to use [SourceTree](https://www.sourcetreeapp.com/) to avoid relying on the console only.

#### Using SourceTree
##### SSH Keys
After installation, you may have to generate a SSH key. Follow [Github's guide](https://help.github.com/articles/generating-an-ssh-key/) for creating one. 

When the key is created, go to SourceTree and select `Tools > Add SSH Key...`. On Windows, your key is stored in `C:\Users\<Username>\.ssh\id_rsa`. 

Upload the contents of the public key (`id_rsa.pub`) to your [Github configuration](https://github.com/settings/ssh/audit).

##### Adding the repository
In SourceTree, go to `File > Clone/New...`.

Enter the following Source Path: `https://github.com/Siipis/Exploration.git`.

Select a Destination Path in your local folders. Note that the folder needs to be empty for the repository to be loaded.

Click `Clone`. The repository should now be visible in SourceTree.

##### Saving your changes in files
Any change you make will become visible in the `Working Copy` tab in SourceTree. Click the checkbox for the files you want to save in the version control and write a Commit message that explains what changes you have done. 

By clicking `Commit` you store the changes in your *local* repository. Changes are not immediately visible to other people.

In order to show your changes to others, use the `Push` icon (blue arrow pointing up) in the top part of the SourceTree window.

##### Short explanation of icons
`fetch` looks for changes in the remote repository, but doesn't download them

`pull` downloads the changes other people have done to the remote repository

`push` uploads your changes to the remote origin

`branch` creates a "spin off" version of the project where you can store changes that are in conflict with the main version. It's a good habit to create your own branch when downloading a repository and upload all your changes there

`merge` combines two branches into one branch


### Installation
You need both Node.js and NW (formerly Node-Webkit) to be present on your computer. 

Start by downloading Node.js [here](https://nodejs.org/en/). It's recommended to use the `v4.2.6 LTS` version.

Download NW [from here](http://nwjs.io/). Select the stable version.

**You may install the programs wherever you like on your computer, as long as you know where to find them.**

### Programming Environment (IDE)
Download [Webstorm](https://www.jetbrains.com/webstorm/). This will be the software you use the most.

Open the project files by selecting `File > Open` and going to the folder where you downloaded the source files. (See SourceTree if you've forgotten.)

#### Running the files
Go to `Run > Edit Configurations...` and click the plus icon to add a new configuration. Select `NW.js` from the list.

Give the configuration a name you recognize. We recommend `Exploration`.

In the `NW.js app` and `Working directory` fields, enter the path to the source files (i.e. the folder you just opened in Webstorm)

In the `NW.js interpreter` field, enter the path to the `nw.exe` you installed in the previous step. 

Click `OK`.

In the top right corner, you should now see the name of the configuration and three icons. To run the file normally, select `Run`. If you wish to have access to the Javascript console and other useful tools, select `Debug` instead. Enjoy!
