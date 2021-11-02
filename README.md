# Making an online resumé

### **Table of contents**
- [Purpose.](#purpose)
- [prerequisites.](#prerequisites)
- [Instructions.](#Instructions)
    - Use a Lightweight markup Language: Markdown
    - Make static websites: Jekyll
    - Use distributed version control: Github Pages
- [More resources.](#More-resources)
- [Authors and acknowledgments.](#Authors-and-Acknowledgments)
- [FAQ.](#FAQ)

### **Purpose**
---
Describe the practical steps of how to host and format a resumé using Markdown, VScode, GitHub Pages, and Jekyll.

### **Prerequisites**
---
- Jekyll.
- VScode.
- A Github account.
- Git installed on your computer.
- A resumé formatted in Markdown.

### **Instructions**
---
 **_a). Use a Lightweight markup Language: Markdown_**

Lightweight Markup Languages such as **Markdown** or ASCIIdoc are an easy-to-learn alternative to other markup languages like HTML or XML. While they do not have as many formatting options as other word processors, it is much more straightforward to collaborate with other individuals because changes can be merged much more easily. Overall, they give you the best of both worlds between nicely formatted text and web portability.

For this tutorial, the lightweight Markup Language we will use is Markdown. To use Markdown. we will need a Markdown editor. The Markdown will be using VSCode.

_Download VSCode_
1. Go to the VSCode website [here](https://code.visualstudio.com).
2. Open the browser's download list and locate the downloaded archive.
Extract the archive contents.
3. Use double-click for some browsers or select the "magnifying glass" icon with Safari.
4. Drag Visual Studio Code app to the Applications folder, making it available in the macOS Launchpad.
5. Add VS Code to your Dock by right-clicking on the icon to bring up the context menu and choosing Options, Keep in Dock.

 **_b). Make static websites: Jekyll_**

Static websites do not have any server-side application dependencies or databases and thus are easy to migrate and they never crash.

Static site generators are tools that help you create your static site. Although you could make a static site without them, they make the task easier by processing everything into a website for you and it is easy to update the site. 

_download Jekyll:_ macOS

1. Check what version of ruby you have installed by typing the command, `ruby -v`, into your terminal. If you do not have ruby installed, you will have to download it.
2. Check what version of gem you have installed by typing the command, `gem -v` into your terminal. If you do not have gem installed, you will have to download it.
3. Type the command `gem install Jekyll bundler` into your terminal to download Jekyll.
4. To ensure that the download worked successfully. Type the command `Jekyll -v` to check the version of Jekyll you have installed.

_create a static site_
1. Open a new folder in VSCode 
2. Type the command `Jekyll new {site name}`In the terminal on VSCode to create some default scaffolding for your site in a new folder. 
3. Copy the content of your resume into the file named `index.md`.
4. Host your brand new site on your own machine using the command `bundle exec jekyll serve`.

 **_c). Use distributed version control: Github Pages_**

Distributed version control is a form of version control in which a project's complete codebase, along with its commit history, can be mirrored on every developer's computer. in contrast to centralized version control, Distributed version control allows automatic management branching and merging, speeds up most operations except "push" and "pull", improves developers' ability to work offline, and does not rely on a single location for its backups.

For this tutorial, we will be using Github for version control and its static site hoster: Github pages. Github pages will allow you to host your resumé online for other people to see.

1. Make a new repository on [GitHub](https://github.com). pick a name for your new repository and ensure that its visibility is set to public.
2. Set the variable `baseurl`, In the `config.yml` file, that Jekyll created to the name of the repository you have just created.
3. Navigate to the directory of your static site in your terminal, 
4. Type the command, `git init` to initialize a local repository. 
5. Type the command, `git checkout -b gh-pages` to check out your gh-pages branch. 
6. Type the command, `git status`. there should be no commits done yet.
7. Type the command `git add.` to add all the files to the local repository. 
8. Type `git commit m {first commit message}`, to commit these files to your repository.
9. Copy the link to your Github repository.
10. Type the command, `git remote add origin {link to your Github repository}` to link your local repository to your Github repository. 
11. Type the command, `git push origin gh-pages` to push all changes made in your local repository to your Github repository. You should see your files in your Github repository.
12. On your Github settings, under the `pages` subsection, there is another subsection called source. Make sure that the branch field is set to the gh-pages branch (_if that is the branch you used_)and the folder is set to the root (_if the files are in your root directory on your repository_).

 **On the same page, near the top, you will notice a banner that says,**

 `Your site is published at HTTPS://{github username}.github.io/{repository name}/`.

 **you may click on that link to view your site.**

![GIFdemo](img/screenrecordddd.gif)

### **More Resources**
---
- A [Markdown Tutorial](https://www.markdowntutorial.com).
- [Modern Technical Writing: An Introduction to Software Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) by Andrew Etter.
- VScode [documentation](https://code.visualstudio.com/docs/languages/markdown) about how to use it with Markdown

### **Authors and Acknowledgments**
---
_Group members: group 8_
- Michael Bathie. 
- Faith De Leon.
- Tuan D. Le. 
- Andy Tan.
- Olukoye Fatoki. 

_Theme authors:_
- [Steve Smith](https://github.com/orderedlist).


### **FAQ**
---
1. Do I need to use VSCode as my Markdown editor?

    - No. Any Markdown editor would probably work the same, if not better than VSCode. It was my personal choice

2. Why is my resumé not showing up?

    - One possible issue is that your Github pages source may not be set correctly. Refer to step 13 under the Instructions subsection, "Host your site on Github pages".

    - Another explanation for this is that your baseurl is misspelled. Refer to step 2 under the Instructions subsection, "Host your site on Github page".