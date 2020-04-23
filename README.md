# Resources
Resources probably has what you need. If something is missing, feel free to add it!

# Contents
* [Rules and Regulations](#RulesandRegs)
* [How to write markdown and README's](#markdown)

# Rules and regulations <a name=RulesandRegs></a>
Here we have the rules and regulations for interacting wiht this repository. Please do not add or remove rules if you are not an admin. These are in place to protect our work.

* Use version control for software projects.

* Do not ever push code to the master branch of important production code.
  * clone the repo and make changes.
  * commit the changes and make a pull request to the development branch.
  * Reviewers will review the changes and merge them.
  * The master branch will be forward facing and only accepted code will be merged on a major releases.
 
* Use appropriate versioning. Major, minor build convention.
  * Add a version tag for production designated with `--version`.
  * eg. 1.2.3:
    * 1 --> First major stable build
    * 2 --> Second major feature addition
    * 3 --> third bug fix
    
* Always fork the repository. Do not download and reupload it as your own.
* Don't remove past members without review. There may be critical builds lost.
      
# How to write markdown documents <a name=markdown></a>
Markdown is a html markup and used to write these readme documnets as well as notebooks. You can also use HTML in markdown and there is some overlap. Interested in HTML, check out [w3scools](https://www.w3schools.com/html/default.asp) for examples. Want a pdf cheatsheet, find it [here](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)

## Something specific?
* [Headers](#header)
* [Lists](#lists)
* [Images](#images)
* [Links](#links)
* [Emphasis](#emphasis)
* [Blockquotes](#blockquotes)
* [Escape](#escapes)
* [Mentions](#mentions)
* [Code blocks](#CodeBlocks)
* [Task lists](#taskList)
* [Tables](#tables)
* [Emoji](#emoji)

## Markdown headers <a name=header></a>
Headers follow the same convention as html `<h></h>` tags, which is replaced with a `#`. As the `#` increases the size of the font will decrease.
```
# This is a Main header
## This is a secondary header
### This is a tertiary header
<h4>Following the same convention using tags</h>
```
# This is a Main header
## This is a secondary header
### This is a tertiary header
<h4>Following the same convention using tags</h>
<br>

## Markdown lists <a name=lists></a>
Lists can be ordered or unordered

#### Ordered list
```
1. Item 1
2. Item 2
3. Item 3
 * Item 3a
 * Item 3b
```
1. Item 1
2. Item 2
3. Item 3
  * Item 3a
  * Item 3b
 
#### Unordered list
```
* Item 1
  * Item 1b
    * Item 1b1
* Item 2
```
* Item 1
  * Item 1b
    * Item 1b1
* Item 2

## Images <a name=images></a>
Images can be references like links but by using a path within the github folder. The difference between linking websites and images is the use of a `!` before the first bracket. This is the syntax to display the logo:
```
![image](/data/0.gif)
```
![image](/data/0.gif)

## Links <a name=links></a>
Generally the same as images and can be used inline as well. Replace the path with your url and remove the exclamation mark. Links can also point internally.

#### The base implementation is done like this:
```
[Link](url)
[link to goolge](https://www.google.com)
```
[link to google](https://www.google.com)

I can also [link to google](https://www.google.com) in text.
#### Place a image using outside links
```
![Link to google](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png)
```
![Link to google](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png)

## Place emphasis on words <a name=emphasis></a>
```
**This will be bold**
__Also bold__
*This is italics*
_Also in italics_
**We** can _mix_ it **up**
```
**This will be bold**
<br>
__Also bold__
<br>
*This is italics*
<br>
_Also in italics_
<br>
**We** can _mix_ it **up**

## Adding blocquotes <a name=blockquotes></a>
Block quotes can be used to highlight paragraphs
```
Sometimes things are better in blocks:

>Here is the start of a block
>but it can be extended easily
>to a new line
```
Sometimes things are better in blocks:

>Here is the start of a block
>but it can be extended easily
>to a new line

