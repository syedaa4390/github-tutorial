# GitHub Tutorial Project

_By Syeda Sabiha Afroj_

---
## Git vs. GitHub
**Git** generally runs around the idea of **version control**. What this means is that it caves ***changes** made   overtime*. Changes based on various commands are able to be tracked because of Git. One thing that doesn’t exist within git is collaboration. Only one person can work on it.

**GitHub** is a website where all your work gets *sent* to a certain **cloud** located there. A **pro** in using GitHub is the ability of **collaboration**. It allows multiple people to work on one repository and send work to each other. This **uses** ***Git***, so it can display the changes being done throughout every commit.

---
## Initial Setup
**maybe add images so these users know what you are talking about**  
The following are instructions on how to create your own Github account...
1. Go to **github.com**
2. Click on **Sign Up** at the top right hand corner of the site.
3. Next, create a **username** and **password**, as well as put in your **HSTAT email**. Your username can be the same as your email.
4. Continue your setup for the Github account.

After, you will have to set up the **SSH feature** in your account. This should only be done **once**. 

It is **important** to do such SSH feature *because* it automatically authorizes you to run your code and display it **efficiently**. This would pretty much speed up your process, since you would no longer have to put in your password in order to verify yourself every time. 

In order to successfully enable this feature, you must do the following steps: 
1. Begin the process by logging into your github account.
2. Next, locate to the **top right hand corner**, where you’ll find your ***profile** icon*. Click on the icon, and then click **Settings** when the list of options appear. Settings should be the **second to last option**.
3. Once you have opened the Settings page, you will see an option that says **SSH and GPG Keys** at the **left sidebar** of the screen. Click on that.
4. When that is done, locate the *green* option that says **New SSH Key** at the **top right hand corner** and click on that.
Once the next page appears, Title it cloud9. As for the key section, do the following:
    * Go to **c9.io** and locate the ***gear** icon* at the **top right hand corner** of the screen, and click on that.
    * Click on the **SSH keys** tab.
    * **Copy** everything that is located in the **second** box, labeled **Connect to your private git repository**.
    * **Paste** all of that copied things into the keys section on the Github page.
6. Click **Add SSH key**.

---
## Repository Setup + Workflow & Commands
Let’s create a new repo (repository)in your GitHub. This can be done through the following commands in such order… 
1. With the **command** `cd ~/workspace` , make sure you are in the accurate working space.
    * `Cd` briefly changes the directory to wherever the user wants to be directed to.
2. By using the **command** `mkdir repo-name` , you will make a directory/repo, with whatever name you desire.
**(explain why it is important to use a dash in a repo name.)**
3. Next, go into that exact directory by the **command** `cd repo-name`.
4. Once that is done, type in the **command** `git init`. This command simply initializes everything in the directory, aka the repository, so that it can be ready for the version control that’ll be done in the future. *Note* : this should only be done **once**.
5. When adding a new file into a repository, you simply do `touch README.md`. *Note* that when `touch` is being used, a new **empty file** is created. In this case, we're always going to be creating an empty file that is name **"README"**.
6. Open up the *README* file by using the command `c9 ` followed by *README.md*, in which case the full command is `c9 README.md`.
7. The three following `add` commands are what makes all your edits ready to be Committed.
    * The command `git add file.ext` adds specific file(s) to the staging area. The part that says *file.ext* is what gets replaced with the actual file names.
    * When using the command `git add .` all the files that had been changed gets added to the directory.
    * Lastly, use `git add --all` when adding *everything* to the staging area. **Everything**  includes all changes, including any deleted files.
8. Now, onto the committing part. When committing a file, the following command would be used : `git commit -m "specific-message"`. This command *finalizes all the changes* that would be made. The part within the quotations are is the message one would be providing. In such message, one should be descriptive towards the specific changes that were made since the last commit.
9. Finally, you have to `push` all your changes into the cloud that's in GitHub. Though, you would need a **remote repo** to push everything to. *Note* that you don't always have to create a remote repository. When it's done once, it's good enough for the rest of the project. A remote repo can be created through the following steps : 
    * Locate to the `+` icon at the top right hand corner of Github, and click on that. Once the options appear, click on the first option that simply says *New Repository*.
    * Rename the repository to whatever is relevant, and **keep the name the same the whole time**.
    * Finalize in creating the repository by clicking *Create Repository* in green.
10. End with the command `git push`.

`Git status` is a very important command that should always be used throughout every changes being made. What `git status` does is simply track the types of changes that would take place, as well as display what type of files are ready to be committed, and if the branch is ready to be committed or not.

---
## Rolling Back Changes
Start off by entering the command `git status`
* In order to **undo** an ***edit***, simply type in the command `git checkout -- filename`. When one doesn't make the proper/desired edit, they can use that command, as if they're going back.
* When one had to undo an `'add`, the commad `git reset HEAD filename` would be useful. Through this command, one can **reset** the added changes.
* As you'd want to undo a `commit`... 
    * you can use the command `git reset --soft HEAD~1`, when you want to undo **only the commit**.
    * you can use the `git reset HEAD~1` command when you want to undo the **commit** *and* the **edit**.
    * you can use the command `git reset --hard HEAD~1` when undoing changes to the **commit, add**, *and* **edit**.



