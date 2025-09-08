# NTNU_TK8117_2025
Common repository for the advanced topics in TK8117
If you donæt have a git user yet, git started now. 

This repository is meant to be a common tool for everyone to colaborate in the advanced topics of TK8117. The idea is to be able to share code from all groups without having to create multiple different git hub repositories. Data can also be included, but GITHUB has ha limit to how much that can be stored, therefore a future potential use of Google drive or similar, could be used.

Each advanced topic has it's own folder, and each folder has it's own set of group subfolders that are free to use. 


# For the people that are unfamiliar with GIT

Git (according to the author) is awesome. It allows for colaboration on code writing across computers and with the ability to branch different versions and merge them into a final version. Additionally there is a complete log over all previous versions of the code (commits).
For more reading on git branches see: https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell

Git is not live coding, but works on a "download-work-upload" concept. Thus if two people work on the same file at the same time, it is not a problem, but needs to be handled with precaution. 


To keep things from beeing messy, here are some rules regarding working with git.
1. Stay to your group's folder, and use a uniqe branch for the group. 
2. Try to keep the work preformed by each person on a separate python file. Makes some potential cleanup redundant.
3. If you are uncertain of where you are in a pull/push situation, create a separate branch and fix afterwards.


# The recomended use of GIT - or how the author likes to use it...

If you prefer to upload, edit and download manually from this webpage, that is fine. For the people who whishes to use the terminal, here is a simple recipie.

1. Download anaconda: https://www.anaconda.com/download. Once downloaded you can find the "anaconda prompt" on your computer, and finish setting up. 
<img width="323" height="69" alt="image" src="https://github.com/user-attachments/assets/2343f14f-7c18-43a9-b1e6-aa986ad3a9e3" />

2. In the anaconda prompt, you can navigate to all folders on your computer using the following commands:<br>

   cd directory_name   to enter a new subfolder, change destination to match the directory<br>
   "cd .." to move one folder up<br>
   "dir" to see the contents of the directory<br>
   "mkdir directory_name" to create a new directory/subfolder, the name can be chosen by replacing "directory_name"

   Try it out and find/create a folder where you can store the work preformed in the course.

4. It is highly recomended to work in virtual environments. https://www.anaconda.com/docs/getting-started/working-with-conda/environments
   Thus you can easily control the packages and the python version needed for any project.

5. Install packages. THis is where the fun begins. If you have worked on an IDE before, you have probably used it to install packages, such as numpy. Now we can do this through the commandline. We can install the first package needed<br>
```
conda install git
```
7. To use github,  it is recomended to onlu download the subfolder needed for your group. Thus you don't end up with 60 subfolders. The recipie for such can be found here: https://medium.com/@marcoscannabrava/git-download-a-repositorys-specific-subfolder-ceeabc6023e2
   <br> the repository url can be found as shown in the following image:
   <img width="1291" height="770" alt="image" src="https://github.com/user-attachments/assets/179755f4-6f93-49b7-9714-638c527a75ae" />

8. You can now work and edit the code on your computer. Most likely using VS code or Jupyter, but more on that later. Let's just assume you've done your work and are now ready to upload it back to the github Repository.
   <br> You can check the status of the files you have modified by typing:
   ```
   git status
   ```
   This will show any changed files in red.
   If you want to add them to the update you are going to upload, type:
   ```
   git add example_name.py
   ```
   If you check the status again, you will se that it is now green.<br>
   When finished adding the nessecary files, you can commit it and write a message:
   ```
   git commit -m "<write your commit message here. WHat was changed and so on. ex: added new features for display>"
   ```
   Then, when all is set and done.
   ```
   git push
   ```
You should now see the update you pushed to the github repository online. 


# The working on the code part and RISE
THere are a couple things needed, primarily, start by installing jupyter notebook and lab as instructed: https://anaconda.org/anaconda/jupyter
Now, RISE is a bit wierd in that the new version of rise, that is compatible with the latest version of jupyter noteook and lab, is not the one the internet points you to. The correct one is here: https://github.com/jupyterlab-contrib/rise.
For the use of rise, see the same url. 

To start jupyter(lab is recomended) from the terminal, make sure to be positioned in the correct folder and type:
```
jupyter lab
```
If everything is done correctly it should work, Remember to save. 
