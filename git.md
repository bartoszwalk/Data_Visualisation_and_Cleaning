# Git

**Summary:** Git is an open source version control system that lets users manage changes to files/directories and collaborate on projects.

**Data formats in:**  Text files (.md, .txt, .py, .js, .html, .css, .r)  
**Data formats out:**  Text files (.md, .txt, .py, .js, .html, .css, .r)

**Three tips:** 
1. If you make a typo in a commit message, *git commit -- amend -m 'new message'* lets you rewrite the message.
2.  To associate a text editor with git on Linux like **VS Code**, you can configure it in your terminal with *git config --global core.editor "code --wait"*. Commands for other editors can be found [here.](https://docs.github.com/en/get-started/getting-started-with-git/associating-text-editors-with-git)
3. You can inspect the changes to a file between the most recent commit and past commits with the command *git diff HEAD\~NUM..HEAD\~NUM FILENAME* where NUM refers to how many commits you want to go back and FILENAME is the file you're inspecting. e.g *git diff HEAD\~1..HEAD\~2 index.html* looks at the difference in index.html between the 2nd and 3rd last commits.

**Examples of use:** ![inspecting changes in file between commits](images/git%20example.png)

**Contribution to data analytics pipeline:** To some extent git can be used in all parts of the data pipeline but in a careful manner. Large datasets should not be contained within git commits themselves as git works best at tracking changes in code or text files, not binary files. Large data-sets could possibly be stored at an external URL. Large output images should also not be stored within commits as that would make the process highly ineffecient. The processing/analysing phases would probably be where git shines with a carefully thought out .gitignore file to ignore large files.

**Comment on your skill level:** My current skill level with git is a 7. I've used git before on personal projects and know the basic workflow. However, I've never used it in a collaborative manner with other people. To get better I'd have to undertake a joint project and practice merging and dealing with conflicts when changes have been made by multiple people.
