# Resources
Resources probably has what you need. If something is missing, feel free to add it!

# Contents
* [Rules and Regulations](#RulesandRegs)
* [How to write markdown and README's](#markdown)
* [Bioinformatics and data science](#bioinfo_ds)
* [Tmux](#tmux)

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
* Readme's should contain the following information:
  * Description of the project
  * Installation instructions
  * Inputs and outputs if neccesary
  * Description or showcase if appropriate
* For open source the default license is GPL v3.0. For permissive licenses we use MIT.
      
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

## Adding blockquotes <a name=blockquotes></a>
Block quotes can be used to highlight paragraphs
```
Sometimes things are better in blocks:

>Here is the start of a blockquote. This formats all of this stuff in a nicer way. 
>Sometimes its all you really need.
```
Sometimes things are better in blocks:

>Here is the start of a blockquote. This formats all of this stuff in a nicer way. 
>Sometimes its all you really need.

## Escaping markdown syntax <a name=escapes></a>
This is a way to write markown documents and still use some of the commonly used characters. Markdown uses the `\` to escape characters and display them as literal.
```
**Not Escaped**
\**Escaped\**
```
**Not Escaped**
<br>
\*\*Escaped\*\*

## Creating code blocks <a name=CodeBlocks></a>
Code blocks create designated space for code which can be used for copy and paste purposes later. Do not write any code that will not run. This is cause for massive frustration down the line. A code block is made with three back ticks on the top of the code and the bottom to end it. adding the language name to the top three back ticks will add syntax formatting.
##### Bash with and without syntax
```
echo ${hello}
```
```Bash
echo ${hello}
```
##### Python
```
import numpy as np
```
```Python
import numpy as np
```

## Task lists <a name=taskList></a>
Task lists create checkboxes to show progress. 
```
- [] I did not do the thing
- [x] I did do the thing
```
- [ ] I did not do the thing
- [x] I did do the thing

## Tables <a name=tables></a>
The most annoying thing to make but it feels good once you are done. Tables are constructed with `|` and `-`
```
|Column1 header|Column2 header|Column3 header                          |
|--------------|--------------|----------------------------------------|
|Thing in col1 |Thing in col2 | Thing in col                           |
|`Formatted`   |**Formatted** |[Link to google](https:\\www.google.com)|
|Thing here    |52668         |![image](/data/0.gif)                   |
```
|Column1 header|Column2 header|Column3 header                          |
|--------------|--------------|----------------------------------------|
|Thing in col1 |Thing in col2 | Thing in col                           |
|`Formatted`   |**Formatted** |[Link to google](https:\\www.google.com)|
|Thing here    |52668         |![image](/data/0.gif)                   |

## Emojis <a name=emoji></a>
In case these are still relevant to use. Its supported. Find all your options [here](https://www.webfx.com/tools/emoji-cheat-sheet/)
```
:+1: :sparkles: :camel: :tada:
:rocket: :metal: :octocat: 
```
:+1: :sparkles: :camel: :tada:
:rocket: :metal: :octocat: 

# Bioinformatics and Data Science <a name=bioinfo_ds></a>
## Links to online resources
|Name      |Description                                             |Citation (if applicable)|
|----------|--------------------------------------------------------|------------------------|
|[Provision](http://provision.shinyapps.io/provision/)|Proteomics data analysis workflow from MaxQuant output. | |
|[Webgestalt](http://www.webgestalt.org/)| Pathway and gene onthology enrichments for model organisms. |[Manuscript](https://doi.org/10.1093/nar/gkz401) |
|[Reactome](https://reactome.org/) | Exploratory pathway enrichment, especially for human. |[Manuscript](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3013646/)|
|[String](https://string-db.org/) | Database of known and predicted protein-protein interactions | [Manuscript](https://www.ncbi.nlm.nih.gov/pubmed/30476243) |
|[Mycobrowser](https://mycobrowser.epfl.ch/) | Collection of mycobacterial genomes and annotations. |[Manuscript](https://doi.org/10.1016/j.tube.2010.09.006) |
|[TB depot](https://depot.tbportals.niaid.nih.gov/#/home) | Large resource for exploring multiple aspects of tuberculosis infection biology. | [Manuscript](https://www.ncbi.nlm.nih.gov/pubmed/31120982) |
|[Uniprot](https://www.uniprot.org/) | Large database for proteome related information, including reference sequences and metadata. | |
|[NCBI](https://www.ncbi.nlm.nih.gov/) | Large database for genome related information, including reference sequences and metadata. | |
|[SRA](https://www.ncbi.nlm.nih.gov/sra) | Submit and extract raw genome sequence data, United States | |
|[ENA](https://www.ebi.ac.uk/ena) | Submit and extract raw genome sequence data, Europe | |
|[PRIDE](https://www.ebi.ac.uk/pride/) | Submit and extract raw proteome data | |
|[ORF finder](https://www.ncbi.nlm.nih.gov/orffinder/) | Find open reading frames. | |

# Tmux or terminal multiplexer cheat sheet <a name=tmux></a>

Tmux is used to create new windows in the command line and detach from those windows. This means you can exit the server and keep a process running. 

## install with apt package manager
```
sudo apt-get install tmux
```

## Most important functions
start new:

    tmux

start new with session name:

    tmux new -s myname

attach:

    tmux a  #  (or at, or attach)

attach to named:

    tmux a -t myname

detach 
```
tmux detach
```
list sessions:

    tmux ls

kill session:

    tmux kill-session -t myname

