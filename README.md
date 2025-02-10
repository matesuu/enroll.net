# The Enrollment Group Project Implementation for Group 6 (CS401-02)

                                                                    0. autogit (OPTIONAL)

If you are unfamiliar to git or Github, here is a list of steps to start! Or Alternatively, you can clone the autogit automation utility by typing the following into your terminal:

git clone https://github.com/matesuu/autogit.git


From here, you can type the following into your terminal to move autogit into your usr/bin directory (macOS and Linux only):

    cd autogit/src
    make
    sudo mv autogit /usr/local/bin

From here, you can automate the use of git when pushing and pulling changes from Github.



                                                                    1. Getting Started


Assuming you have git installed (if not then refer to https://git-scm.com/book/en/v2/Getting-Started-Installing-Git),
start by typing in the following commands in your terminal application (macOS and Linux):

    git clone <GITHUB_URL> // clones our remote repository on Github.com to your local device

For this project, we will be pushing all changes to a secondary branch called "feature". This is because it will allow us to add changes to a test branch for the sake of unit testing before we merge our final changes into our projects "main" branch. Type:

    git checkout -b feature




                                                                    2. Adding and Pushing Changes

To push all changes that you have made to your files (be careful before pushing!) type the following:

    git add . --all
    git commit -m "<ENTER A COMMIT MESSAGE HERE>"
    git push -u origin feature

After this, you should see all changes made to your files on the most recent commit to the "feature" branch.
If an error message along the lines of "could not push refs", type the following:

    git pull --rebase origin feature

This should fix the issue.








