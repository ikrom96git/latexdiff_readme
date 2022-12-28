# Welcome to Latexdiff!

This is a project to demonstrate how to make use of the git pipeline to create a pdf showing all
changes that were made with respect to some earlier commit. This is done with the help of latex diff.
The default is set to produce the difference between the current commit and
the penultimate change in the latex file.
In order to manually set which two versions should be compared one get set
the variable via the push command.

##  Important

- You need to change directory and file name if it is different from **cwd** and **main.tex**
  >  It can be changed in the following .github-ci.yml file. 
  
  >  Location: .github/workflows/.github-ci.yml
-  Only changes have to be done:
   > env:
   
    > \# Edit here with the names of your latex file and directory (can use ".")
   
	>>DIR: .
	
    >>    FILE: main
    
 - Needs to be change the link to the pdf files in README.md file:
   > \{https://github.com/**username**/**repository_name**/raw/build/**main_tex_name**.pdf}
   
   >https://github.com/**username**/**repository_name**/raw/build/diffversion.pdf
## THE OUTPUT
Here is the current pdf:

[![](https://img.shields.io/badge/Download-pdf-red)](https://github.com/ikrom96git/latexdiff_readme/raw/build/main.pdf)

Here is the version showcasing all the difference to the penultimate commit

[![](https://img.shields.io/badge/Download-pdf-red)](https://github.com/ikrom96git/latexdiff_readme/raw/build/diffversion.pdf)
