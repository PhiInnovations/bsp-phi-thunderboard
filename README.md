Thunderboard's Yocto BSP
========================

This project is based on Freescale's Community Yocto BSP, adapted to build
Thunderboard board.

To get the BSP you need to have `repo` installed and use it as:

Install the `repo` utility:

 $: mkdir ~/bin

 $: curl http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo

 $: chmod a+x ~/bin/repo

Download the BSP source:

 $: PATH=${PATH}:~/bin

 $: mkdir bsp-phi-thunderboard

 $: cd bsp-phi-thunderboard

 $: repo init -u https://github.com/PhiInnovations/bsp-phi-thunderboard -b dora

 $: repo sync

Once this has complete, you will have all you need. To start a build, do:

 $: source ./setup-environment build

You can use any directory to host your build.

The source code will be checked out at bsp-phi-thunderboard/sources.
