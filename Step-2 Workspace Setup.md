//Open cmd as admin

  * wsl

  //wsl opens up
  
  * pwd

  //make sure you are in linux fie system root directory and not in windows local disk mnt

  * uname -a

  //shows some user details

  * sudo apt update
  
  * sudo apt upgrade -y

  //Update and upgrade the system before further progress

  //Now for the project building purposes we need some tools to work with: Use this command:
  * sudo apt install -y \
      git \
      curl \
      wget \
      zip \
      unzip \
      python3 \
      python3-pip \
      make \
      cmake \
      ninja-build \
      bc \
      bison \
      flex \
      libssl-dev \
      libelf-dev \
      build-essential \
      ccache \
      rsync \
      device-tree-compiler \
      lz4 \
      cpio

  //This will install all the necessary tools. Copy paste the entire command on to the wsl terminal

    * pwd

  //make sure you're in the root directory of linux filesystem
  //Now we are going to make the file structure to store our project\
  
    * mkdir -p ~/KernelWorkspace
    
    * cd ~/KernelWorkspace
    
    * mkdir source
      mkdir toolchains
      mkdir output
      mkdir patches
      mkdir scripts
      mkdir docs
      mkdir releases
      mkdir AnyKernel3

    * tree ~/KernelWorkspace
        //expected output:
          /home/ychuu/KernelWorkspace
            ├── AnyKernel3
            ├── docs
            ├── output
            ├── patches
            ├── releases
            ├── scripts
            ├── source
            └── toolchains

      //Next step is version control of our project using GIT
