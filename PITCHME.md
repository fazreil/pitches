---

# Version Control Systems

---

## What is version control system

+++

> A component of software configuration management, version control / revision control / source control, is the management of changes to documents, computer programs, large web sites, and other collections of information.
@div[right-50]
Wikipedia
@divend

+++

> Version control systems are a category of software tools that help a software team manage changes to source code over time.
@div[right-50]
Atlassian 
@divend

+++

### Where VCS sits in Software Engineering pool of tool?

[DevOps periodic table by Xebialabs](https://xebialabs.com/assets/files/infographics/periodic_table_11x17inc_v2_clean_outlines.pdf)

+++?images=assets/images/xebialabs_periodic_table.png&size=auto
@title[Devops Periodic Table]

---

## Types of version control systems

There are two types of Version Control System:
  - Centralized VCS
  - Distributed VCS

+++

### Centralized VCS

  - Logs changes in the @color[#e49436](central) server.
  - Less @color[#e49436](conflicts).
  - Easy to @color[#e49436](administer).

+++

### Distributed VCS

  - Keep the changes in its  @color[#e49436](local repository).
  - Enable work to be carried out @color[#e49436](offline).
  - Cultivate the culture of @color[#e49436](open source).

+++?image=assets/images/centralized-vs-distributed.png&size=75%
@title[Infographic centralized vs distributed VCS]

---

## Popular Version Control System

+++

### GIT

  - Distributed VCS.
  - Biggest user base.
  - Has a @color[#e49436](lot of commands) to manipulate git.

+++

### SVN and CVS

  - Centralized VCS.
  - Pre-Git users are used to Subversion/SVN.
  - Most @color[#e49436](straight forward approach) in Version Control System.
  - Uses trunk, branch, tag approach.

+++

### Clearcase

  - Centralized VCS.
  - A VCS backed by @color[#e49436](IBM).
  - Visually interesting, uses config spec which produce a comprehensive set of files.

+++

### mercurial

  - Distributed VCS.
  - Fast, written in @color[#e49436](python) (platform independent).
  - Claim to have behavior similar to SVN. Migrating to mercurial would be easy.

---

## Common philosophy of a VCS

+++

### Repositories

  - Repositories are basically the @color[#e49436](storage space) to place the content.
  - Repositories shall store files @color[#e49436](relevant) to itself.
  - Sometimes repositories sharing do happen, then it gets confusing.
  - A repository is usually @color[#e49436](invisible) to other repositories.

+++

#### The following slide show a process of cloning a repository
@title[Process of cloning]
  - The process show the @color[#e49436](address) of the git repository.
  - The address is also refers to as @color[#e49436](remote url).
  - Default remote url is called @color[#e49436](origin).
  - @color[#e49436](git status) shows which branch you are in.

+++?image=assets/images/git-clone.png&size=75%

@title[Cloning a repo]

+++

### Branches and Tags

  - Branches are a @color[#e49436](stream of work).
  - Multiple branches allow work to be done @color[#e49436](in parallel).
  - Some branches are meant to be read only, these are called @color[#e49436](Tags).
  - Tags freeze the file at a certain point. the point refers to a commit.

+++

#### The following slide show the collection of branches both available locally and remotely
@title[Collection of branches]
  - The lines starting with 'remote' are branches available in @color[#e49436](remote repo).
  - If there are remote branches listed that is not available locally, you are @color[#e49436](not tracking) the branch.

+++?image=assets/images/git-local-remote-branch.png&size=75%

@title[Git local and remote branches]

+++

### Commits

  - Commits are @color[#e49436](transaction) of changes made by an author.
  - A commit may contain one or more @color[#e49436](changes) across the files.
  - A commit marks a new @color[#e49436](revision/version) that add up to the current branch. 

+++

#### The following slide show the status of the git repository
@title[Status of the git repository]
  - It shows @color[#e49436](how your branch is doing) compared to the origin.
  - It also list down @color[#e49436](modifications) made with the content.
  - New files @color[#e49436](not yet tracked) by the repo is shown here too.

+++?image=assets/images/git-status.png&size=75%

@title[git status]

+++

### Logs

  - List of commits.
  - May show the @color[#e49436](relation between branches).
  - Useful to show @color[#e49436](the work done) for certain file.

+++

#### The following slide show a log of work done on a file
@title[Log of work done on a file]
  - It shows @color[#e49436](who do what).
  - It also show what was the @color[#e49436](commit message).
  - It shows @color[#e49436](what time) it was done.

+++?image=assets/images/log-file.png&size=75%

@title[Git log file]


+++

### Diff

  - A diff is a @color[#e49436](comparison) between two commits.
  - A diff can also be a comparison between an @color[#e49436](unstaged) and a @color[#e49436](versioned) files.
  - Useful when trying to figure out what happened between commits.

+++

#### The following slide shows an example of a diff
@title[Example of a diff]
  - It shows @color[#e49436](what files) being diff.
  - You can see what was added (@color[green](+)) and what was removed (@color[red](-)).
  - This helps you look at @color[#e49436](what have you worked) on.

+++?image=assets/images/diff.png&size=75%

@title[Git diff]

+++

### Merging

  - Merging is an act of @color[#e49436](combining) the content of two branches.
  - Modern tools usually have @color[#e49436](auto merging) feature built in.
  - Manual merge is required when there are @color[#e49436](conflicts) arise during merge.
  - Manual merging is a process of @color[#e49436](picking relevant changes) into the branch.

+++

#### The following slide show a log with branches and merging happening
@title[Branches and merging]
- It shows @color[#e49436](what was done) on which branch.
- And show what was contributing to each branch.
- Tells how it relate to other branches, like @color[#e49436](branching) out and @color[#e49436](merging) in.

+++?image=assets/images/log-branches.png&size=75%

@title[Git log branches]


---

## VCS server and client

+++

### Clients for Windows

+++?image=https://i.stack.imgur.com/jhnqO.png&size=auto
#### @color[#e49436](tortoise git)

+++?image=http://wiki.eclipse.org/images/d/d3/Egit-0.11-getstarted-compare.png&size=auto
#### @color[#e49436](Eclipse EGit)

+++

### Clients for Mac

+++?image=https://images.filehippo.net/img/ex/6696__sourcetree_1_23_2_16.png&size=auto
#### @color[#e49436](Sourcetree for MAC)

+++?image=https://tower-website-ftkdppxp1xaznovg.netdna-ssl.com/assets/img/screenshots/largeScreen/mac/working-copy_a.png&size=auto
#### @color[#e49436](Git Tower for MAC)
+++

### Clients for linux

+++?image=http://mkjblogs.com/wp-content/uploads/2016/03/gitCola.jpeg&size=auto
#### @color[#e49436](Git Cola)

+++
#### To be honest if you are on linux chances are you'll be loving working on the @color[#e49436](terminal)
@title[IMHO]

---

## Practical use of VCS


+++

### Update your code frequently
  - To avoid conflicts, update code frequently.
  - It will be best to work on the latest code.
  - Conflicts might are not just at the code level, but branch level.

+++

### Manage conflicts diligently
  - Keep changes to their respective commits.
  - If there are multiple changes that are irrelevant to each other, it will be hard to manage the commits.

+++

### Commit relevant changes with relevant message
  - Best to group a commit to relevant files being modified.
  - while committing a bunch of files is easy, committing the files with common commit makes the log more readable.

+++

### VCS is not just for coding
  - VCS can be utilised to record changes of files.
  - Work best with plaintext.
  - Can also work with keeping configuration files of applications.
  - These slides are produced with GIT.
  

---  

## Q&A