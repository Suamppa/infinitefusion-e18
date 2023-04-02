# How to contribute to Infinite Fusion
_Notice: These instructions are written by a contributor who learned this through trial and error. Easier methods and other changes can and should be edited in._

***This document assumes that you have some basic development setup already in place***

## Prerequisites
1. Git
2. RPG Maker XP
3. Visual Studio Code or some other IDE (optional, but recommended)

## Getting started

### Quick setup (playtesting will not work)
1. Fork the repository
2. Clone the repository to your computer into an empty folder
3. Get the main Infinite Fusion download from the official source and extract normally
4. Place the cloned repository on top of the game files and overwrite when prompted
5. Open RPG Maker XP
6. Make a new empty project and save it
7. Go to the project location and copy the `Game.rxproj` file into the Infinite Fusion game folder
8. You can now open this project file in RMXP to edit Infinite Fusion
    - Playtesting will not be functional (`Failed to create process.`)

### Complete setup
1. Fork the repository
2. Clone the repository to your computer into an empty folder
3. Download Pokemon Essentials (the whole thing, not the repository)
4. Either extract Pokemon Essentials into the cloned IF repository and *don't* let it overwrite any files (I have not tested this) or extract it normally into the folder you want to use for development and then copy and paste in the cloned Infinite Fusion repository, overwriting files when prompted
5. Remove non-Infinite Fusion files...
    - with Visual Studio Code:
        1. Open the folder in VSCode
        2. Open the source control tab
        3. Stash or discard changes
            - Because the repo is cloned from GitHub, this will only stash or discard extra files brought in by Pokemon Essentials that Infinite Fusion does not use
    - with Git Bash:
        1. Open the folder in Git Bash
        2. Enter `git stash --keep-index --include-untracked`
6. If you want to edit scripts, it's highly recommended to [install Ruby](https://www.ruby-lang.org/en/)
    - Recommended VSCode extensions: Ruby, Ruby Solargraph, ruby-rubocop (rubocop will cause messy commits because of auto-formatting, but it would help clean up the scripts over time if you want to use it)
