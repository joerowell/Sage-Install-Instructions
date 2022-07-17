# Installing Sagemath for great good
This document is meant to provide some brief instructions on how to install Sagemath on your device in preparation for the lattice labs.
Please note that it's impossible for us to cover all possible combinations of operating systems and hardware: as a result, we only attempt to cover
the most common cases here. If you have a combination that isn't covered in this document, feel free to reach out to the organisers: we will try our best to help.


## Sagemath on Linux
Sagemath is provided by the package managers of most linux distributions. Thus, installing Sagemath is normally as simple as typing something like this in your terminal:

```bash
sudo apt-get install sagemath # On Debian or Ubuntu
```

Depending on your operating system you'll likely need to substitute the call to ```apt-get install``` with the specific syntax for your package manager: you'll likely know the
syntax far better than we do.

## Sagemath on Macos.
Sagemath can be installed on Macos in a few ways. Here we will focus on two: using [Brew](https://brew.sh/), and using [Conda](https://docs.conda.io/en/latest/).
We recommend using Brew, as it is slightly easier to use compared to Conda.

### Using Brew
[Brew](https://brew.sh/) is a package manager for Macos. It's a commonly used piece of software that makes it easy to install software on a Mac.
To install Brew, click one of the [links](https://brew.sh/) to Brew and copy the command in the "Install Homebrew" textbox into your terminal.

Once Brew has been installed, you can install Sagemath by typing ```brew install --cask sage``` into your terminal. This may take a while.

After this, you should be able to launch Sagemath by typing ```sage``` into your terminal.

### Using Conda
If you don't use Brew as a package manager, then a nice way to install Sagemath is to use [Conda](https://docs.conda.io/en/latest/). Conda is another package manager for MacOS, but Conda
can also be used on Windows and Linux too. For the sake of this tutorial, we'll use Miniconda, which is a variant of Conda.

To install Conda:
1. Click on [this](https://github.com/conda-forge/miniforge#miniforge3) link and download the right script for your architecture. If your Mac is a new M1 mac, then click on the "arm64" link.
   Otherwise, click on the "x86_64" link.
2. Open your terminal and navigate to your Downloads folder (e.g by typing ```cd ~/Downloads```).
3. You may need to mark the script as executable. To do this, type ```chmod +x <name of the script that was downloaded>```.
4. Install this script by typing ```./<name of the script that was downloaded>```. It's OK to accept all of the default options.
5. Close your terminal and re-open it. When your terminal re-opens, your prompt should start with a ```(base)```.

   
To install Sagemath:
1. Type ```conda create -n sage```. Accept the packages that Conda wants to install.
2. Type ```conda install -c conda-forge sage```. Again, accept the packages that Conda wants to install.
3. Once the installation has finished, type ```conda activate sage```. You will need to do this each time you want to use Sagemath.
4. Finally, to use sagemath, type ```sage```. 


## Sagemath on Windows
Installing Sage on Windows can be a little bit tricky. This is because certain functionalities that Sage depends on aren't necessarily available on Windows.
The recommended way of getting around this is to use the [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/about).

To make this process easier, we have written a installation script for you, along with some instructions.
The script (along with the instructions) can be found [here](https://github.com/joerowell/WSL-for-fplll).


