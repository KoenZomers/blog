# Contributing guidelines

We love to have your contributions! To author a blog post, follow these steps:

1. Register for a [GitHub](https://github.com) account in case you don't already have one - it's free!
2. Install Git for Windows (if you work on a macOS, download Git for macOs). To continue with Windows,

   * Open [Git for Windows](https://git-scm.com/download/win)
   * Download the latest version (64-bit or 32-bit).
   * Optional: If you are not sure what you need, you can check it:
       * Press WIN key and type about
       * Select about your PC, it shows you the System type in the device specifications
   * Open the downloaded file
   * Confirm the User Account Control window by selecting **Yes**
   * In the Git Setup window, select **Next** for 6 times, Git will now extract the files
   * Select **Finish**

3. Install [Visual Studio Code](https://code.visualstudio.com/)

4. Create a Git (not GitHub) account

   * Open the terminal in Visual Studio Code
   * Type `git --version` in a directory of your choice - you should see the version of Git that you downloaded. If you see an error, close and reopen VS Code and try again.
   * Set your user name with 
   `git config --global user.name "<your-first-name> <your-last-name>"` - replace the `<placeholders>` with the real values
   * Set your email address with 
   `git config --global user.email "<your-email-here>"`- replace the `<placeholder>` with the real values (your email address should match the one with which you signed up for your GitHub account)

5.  Fork this repository to create a copy in your GitHub account:

    * Open [pnp/blog/](https://github.com/pnp/blog/) (this repository)
    * Select **Fork** --> The URL of your fork is now `https://github.com/<YOUR GITHUB ACCOUNT>/blog/`

6. Clone the repository

Now you want to clone the repository so you have it locally available:

![fork repository](blog/assets/GitHub-forkclone.png)

* Select **Code**
* Copy the URL (it is `https://github.com/<YOUR GITHUB ACCOUNT>/blog.git`)
* Open the terminal in VS Code
* Navigate to a directory where you want to clone the repository
* Type `git clone <COPIED URL HERE>`

7. Add Upstream

You will now want to make sure, that all your contributions point to the original repository, which is why you want to add an upstream to it:

* Navigate to the folder where your cloned repository is located with `cd blog`
* type `git remote add upstream https://github.com/pnp/blog` (this needs to be the original repository URL)
* to check if everything works correctly, type `git remote -v`, you should see this output:

```powershell
origin  https://github.com/<YOUR ACCOUNT HERE>/blog.git (fetch)
origin  https://github.com/<YOUR ACCOUNT HERE>/blog.git (push)
upstream https://github.com/pnp/blog (fetch)
upstream https://github.com/pnp/blog (push)
```

8. Write your blog post

* type `code .` in VSCode terminal (yes, there is a space (` `) between `code` and the `.`) to open your project in a new VS Code instance
* in the **blog/content/posts** folder, create your own folder (you may use the title of your post as the name of the folder, use `-` instead of ` `)
* in the newly created folder add an `index.md` file with your post.
* create a new folder **images** in your posts folder. In the images folder you may save any image/graphic which may be used in your article
* upload all images for your article in this folder
* in case you need some help on how markdown works, please see this article:
  
[What's up with markdown?](content/post\what-s-up-with-markdown.md)

We also put together some information about markdown and how to use it in our [Wiki](https://github.com/pnp/blog/wiki/Microsoft-365-blog-Markdown-reference)

9. Commit and push your changes to your fork

Whenever you want to upload your changes to your remote fork:

* type `git add .` (yes, there is a space (` `) between `add` and the `.`) - this adds all changes to staging area
* type `git commit -m "YOUR COMMIT MESSAGE"` - this will commit your changes with the messages
* type `git push` to push the changes to your remote fork

10. Pull request

You will now want to (kindly) ask the repository maintainers to pull in your changes. You do that with a pull request:

* Open [pnp/blog](https://github.com/pnp/blog) (this repository)
* Select **Pull requests**
* Select **New pull request**

![create pull request](blog/assets/GitHub-newPR.png)

* Select **compare across forks**
* Select your fork from the **head repository**

![compare changes](blog/assets/GitHub-createPR.png)

* Select **Compare & pull request**

* Fill out the form (please read carefully, this way we don't need to go back and forth too often)
    * give your PR a descriptive title
    * describe what's in the PR (new article with images)
    * provide us with your twitter handle and a short text how we can promote your article. Including your own twitter handle this text can't be longer than 257 characters.
* You can always switch to **Preview** to see how it looks like
* Select **Create pull request**
* If needed, you can commit more files and changes

A maintainer will review your pull request and merge your changes soon so that your blog appears on the [Microsoft 365 Community blog](https://pnp.github.io/blog/).

This repository is maintained by volunteers in their free time, please be kind. Everyone is doing their best to keep things moving forward.

{::ignore rule="MD013" relative_line="-2"}
_Sharing is Caring_
