---

# Version Control Systems

---

## What is version control system

> A component of software configuration management, version control, also known as revision control or source control, is the management of changes to documents, computer programs, large web sites, and other collections of information.
@div[right-50]
Wikipedia
@divend
---

## What is version control system
> Version control systems are a category of software tools that help a software team manage changes to source code over time.
@div[right-50]
Atlassian 
@divend
---

## Types of version control systems

There are two types of Version Control System:
  - Centralized VCS
  - Distributed VCS

+++

### Centralized VCS

@ul
  - logs changes in the @color[#e49436](central) server.
  - less @color[#e49436](conflicts)
  - easy to @color[#e49436](administer)
@ulend

+++

### Distributed VCS

@ul
  - keep the changes in its  @color[#e49436](local repository)
  - enable work to be carried out @color[#e49436](offline).
  - Cultivate the culture of @color[#e49436](open source)
@ulend

+++?image=assets/images/centralized-vs-distributed.png

### Centralized vs Distributed VCS



---

## Popular Version Control System

+++

### GIT

  - Distributed VCS
  - biggest user database
  - Has a @color[#e49436](lot of commands) to manipulate git.

+++

### SVN and CVS

  - Centralized VCS
  - pre-Git users are used to Subversion/SVN
  - most @color[#e49436](straight forward approach) in Version Control System
  - uses trunk, branch, tag approach.

+++

### clearcase

  - Centralized VCS.
  - a VCS backed by @color[#e49436](IBM).
  - visually interesting, uses config spec which produce a comprehensive set of files

+++

### mercurial

  - Distributed VCS.
  - Fast, written in @color[#e49436](python) (platform independent)
  - claim to have behavior similar to SVN. Migrating to mercurial would be easy.

---

## Common philosophy of a VCS

+++

### Repositories

  - Repositories are basically the @color[#e49436](storage space) to place the content.
  - Repositories shall store files @color[#e49436](relevant) to itself
  - sometimes repositories sharing do happen, then it gets confusing.
  - a repository is usually @color[#e49436](invisible) to other repositories

+++

### Branches and Tags

  - Branches are a @color[#e49436](stream of work)
  - Multiple branches allow work to be done @color[#e49436](in parallel)
  - some branches are meant to be read only, these are called @color[#e49436](Tags)
  - Tags freeze the file at a certain point. the point refers to a commit
   
+++

### Commits

  - commits are @color[#e49436](transaction) of changes made by an author
  - a commit may contain one or more @color[#e49436](changes) across the files
  - a commit marks a new @color[#e49436](revision/version) that add up to the current branch 

+++

### Diff

  - a diff is a @color[#e49436](comparison) between two commits
  - a diff can also be a comparison between an @color[#e49436](unstaged) and a @color[#e49436](versioned) files
  - useful when trying to figure out what happened between commits

+++

### Merging

  - merging is an act of @color[#e49436](combining) the content of two branches
  - modern tools usually have @color[#e49436](auto merging) feature built in.
  - manual merge is required when there are @color[#e49436](conflicts) arise during merge
  - manual merging is a process of picking relevant changes into the branch

+++

### logs

  - 

---

## VCS server and client

+++

### clients for windows

+++

### clients for mac

+++

### clients for linux

---

## Practical use of VCS


+++

### update your code frequently
  - To avoid conflicts, update code frequently
  - it will be best to work on the latest code
  - conflicts might are not just at the code level, but branch level

+++

### manage conflicts diligently
  - Keep changes to their respective commits
  - if there are multiple changes that are irrelevant to each other, it will be hard to manage the commits

+++

### commit relevant changes with relevant message
  - Best to group a commit to relevant files being modified.
  - while committing a bunch of files is easy, committing the files with common commit makes the log more readable.

+++

### VCS is not just for coding
  - VCS can be utilised to record changes of files.
  - Work best with plaintext.
  - Can also work with keeping configuration files of applications.
  - These slides are produced with GIT
  

---  

Q&A