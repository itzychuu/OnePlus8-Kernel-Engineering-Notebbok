//make sure git is installed

  * git --version

//configure git using these commands

  * git config --global user.name "username"\
  
  * git config --global user.email "email address"

  * git config --list

   //Should show you username and email

//Go to our project main folder

  * cd ~/KernelWorkspace

  * git init
    //initialized git repo

  * nano .gitignore
    //Paste this content:
    
          output/
          *.img
          *.zip
          *.log
          *.o
          *.a
          *.ko
          *.dtb
          *.dtbo
    
    //To save it:
    
      * Ctrl + O
      * Enter
      * Ctrl + X
    
  // To check the file

    * cat .gitignore

  //Now add and commit the work we did till now using these commands

    * git add .
    
    * git commit -m "Intital kernel workspace"
