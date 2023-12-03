# Welcome to Latexdiff!

This project demonstrates how to use the Git pipeline to create a PDF showing all changes made in comparison to some earlier commit, leveraging latexdiff.

The default setting is to produce the difference between the current commit and the penultimate change in the LaTeX file.

To manually set which two versions should be compared, one can set the variable via the push command.

##  Important

- You may need to change the directory and file name if they are different from **cwd** and **main.tex**.
  > It can be changed in the following .github-ci.yml file.
  
  > Location: .github/workflows/.github-ci.yml

- The only changes that need to be made:
  > ```yaml
  > env:
  >   # Edit here with the names of your LaTeX file and directory (can use ".")
  >   DIR: .
  >   FILE: main
  > ```

- Update the links to the PDF files in the README.md file:
  > [Download Main PDF](https://github.com/username/repository_name/raw/build/main.pdf)
  
  > [Download Latex Diff PDF](https://github.com/username/repository_name/raw/build/diffversion.pdf)

## THE OUTPUT
Here is the current PDF:

[![](https://img.shields.io/badge/Download-pdf-red)](https://github.com/username/repository_name/raw/build/main.pdf)

Here is the version showcasing all the differences to the penultimate commit:

[![](https://img.shields.io/badge/Download-pdf-red)](https://github.com/username/repository_name/raw/build/diffversion.pdf)
