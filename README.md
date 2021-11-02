## HOSTING A RESUME ON GITHUB PAGES

### **Purpose**

Describe the practical steps of how to host and format a resume using Markdown, VScode, GitHub Pages, and Jekyll.

### **Prerequisites**

- jekyll
- VScode
- a resume formatted in markdown

**Instructions**

_Download VSCode:_ 

1. go to the VSCode website [here](https://code.visualstudio.com).
2. Open the browser's download list and locate the downloaded archive.
Extract the archive contents. 
3. Use double-click for some browsers or select the 'magnifying glass' icon with Safari.
4. Drag Visual Studio Code.app to the Applications folder, making it available in the macOS Launchpad.
5. Add VS Code to your Dock by right-clicking on the icon to bring up the context menu and choosing Options, Keep in Dock.

_download jekyll:_ macOS

1. Check what version of ruby you have installed by typing the command, "ruby -v", into your terminal. if you do not have ruby installed, you will have to download it.
2. Check what version of gem you have installed by typing the command, "gem -v" into your terminal. if you do not have gem installed, you will have to download it.
3. Type the command "gem install jekyll bundler" into your terminal to download jekyll. 
4. To ensure that the download worked successfully. type the command "jekyll -v" to check the version of jekyll you have installed.

_make a local site with jekkyll_
1. In VSCode, open a new folder. 
2. In the terminal on VSCode, type the command "jekyll new {site name}" to create some default scsffolding for your site in a new folder. 

_Write your resume in markdown_


_Host your site on github pages:_

1. Make a new repository on [GitHub](https://github.com). pick a name for your new repository and ensure that that its visibility is set to public.
2. set the variable "baseurl", In the "config.yml" file, that jekyll created to the name of the repository you have just created. 
3. Navigate to the directory of your static site in your terminal, 
4. Type the command, "git init" to initialize a local repository. 
5. Type the command, "git checkout -b gh-pages" to check out your gh-pages branch. 
6. Type the command, "git status". there should be no commits done yet.
7. Type the command "git add ." to add all the files to the local repository. 
8. Type "git commit m '{first commit message}"', to commit these files to your repository.
9. Copy the link to your github repository.
10. Type the command, "git remote add origin {link to your github repository}" to link your local repository to your github repository. 
11. Type the command, "git push origin gh-pages" to push all changes made in your local repository to your github repository. 
12. On your github settings, under the pages subsection, near the top, you will notice a banner that says " Your site is published at https://{github username}.github.io/{repository name}/". you may click on that link to view your site.

![GIFdemo](img/screenrecordddd.gif)

**More Resources**

- [This](https://www.markdowntutorial.com) is a markdown tutorial
- [This](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) a book about software documentation.
<!-- - one other resource -->

**Authors and Aknowledgements**

_group members:_
- Michael Bathie. 
- Faith De Leon.
- Tuan D. Le. 
- Andy Tan.
- Olukoye Fatoki. 

**FAQ**

1. Why is Markdown better than a word processor?

- Although a word processor is slightly easier to write in,
(2) Aquestionaboutthepracticaldetails,suchas“Whyismyresumenotshowingup?”
1. Do I need to host my site on the "gh-pages" branch?

- No. you can 

2. what is VSCode?\
- Visual Studio Code is a lightweight but powerful source code editor which runs on your desktop and is available for Windows, macOS and Linux. It comes with built-in support for JavaScript, TypeScript and Node.js and has a rich ecosystem of extensions for other languages (such as C++, C#, Java, Python, PHP, Go) and runtimes (such as .NET and Unity). 