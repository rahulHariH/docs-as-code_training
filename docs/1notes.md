
## Link syntax


link to heading on the same page:
[linkText](#Heading)

## Image syntax

markdown tag:
![imageIdentifierName](/imageFolder/imageName.png)
html tag:
<img src="imageFolder/imageName.png" width="300" height="200" />

## Table syntax

| colHdr1 | colHdr2 | colHdr3 |
| :- | :-: | -: |
| item1  | item2 | item3 |
| leftAlignedText | centreAlignText | rightAlignText |


| colHdr1 | colHdr2 |
| - | - |
| *Stem sentence*:  <ol> <li>First nested item</li>  <li>Second nested item</li>  </ol>   | Text |
| Paragraph </br> next line  </br>next next line | Text |


## Admonitions (Alerts in GitHub)

> [!NOTE]
> noteText

> [!TIP]
> tipText

> [!WARNING]
> warningText

> **Note:**
> Install the software before adding the file.


## TOC syntax

search for TOC in the search bar and pick the TOC. it's basically multiple link in same page macros for all the headings in the page.

## Task list syntax

- [x] Set up the editor
- [x] Write some markdown
- [ ] Connect a cloud service
- [ ] Export the finished document

## Footnote syntax

**1 footnote:**
Markdown is a lightweight markup language.[^1]
 
[^1]: Markdown was created by John Gruber and Aaron Swartz.

**multiple footnotes:**
Markdown is commonly used for documentation.[^1]
GitHub supports GitHub FlavoredMarkdown (GFM).[^2]
 
[^1]: Markdown is designed to be easy to read and write.
[^2]: GFM extends standard Markdown with additional features.

## Expand macro (collapsible) syntax 

<details> 
<summary>Click to expand</summary>
 
//add `open` after `details` and the expander will be open by default//

This content is hidden by default.
 
You can include following types of content:
 
- Text
- Lists
- Code
- Links
- Images
 
</details>


## Git commands

git add .
Adds all your changes to the staging area.
 
git commit -m "commitMessage"

git add
Add a file that is in the working directory to the  staging area (also called "index")

git commit
Add all files that are staged to the local repository

git push
Add all committed files in the local repository to the remote repository
In the remote repository, all files and changes will be visible to anyone with access.

git fetch
Get files from the remote repository to the local repository but not in the working directory

git merge
Get the files from the local repository to the working directory

git pull
Get files from the remote repository directly into the working directory. 
It is equivalent to a git fetch + git merge.

git clone --branch my-branch --single-branch https://github.com/bmc-izot/izot-ix.git

modifying a committed (staged) file | pulls it back from the commit stage
git commit --amend -m "amendMsg"

creating a new branch
git switch -c branchName

switch to main branch
git switch branchName

 