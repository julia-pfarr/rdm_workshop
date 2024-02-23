# Version Control and Provenance Tracking

!!! abstract "Objectives📍"

    - different version control systems and levels
    - motivation for using version control
    - version control with Git
    - versioning data

## Summary

No matter how your group is organized, the work of many contributors needs to be managed into a single set of shared working documents.
Management of changes or revisions to any types of information made in a file or project is called versioning.

In particular, reproducibility requires the provision of **the code and the data** that was used to produce a figure.
In practice, data and code are modified regularly and one needs to record what was changed when, in order to provide provenance information. 
As we will see in this chapter, version control has a lot of other advantages, which explains why most data science project are hosted on Git platforms.

**Version control is an approach to record changes made in a file** or set of files over time so that you and your collaborators can track their history, review any changes, and revert or go back to earlier versions. 
Management of changes or revisions to any types of information made in a file or project is called versioning.
For example, when writing a paper with multiple collaborators, version control can help track what changed, who changed them, and what updates were made.

<figure markdown="span">
  ![Project History](assets/images/ProjectHistory.jpg){ width="600" }
  <figcaption>_The Turing Way_ project illustration by Scriberia. Used under a CC-BY 4.0 licence. DOI: [10.5281/zenodo.3332807](https://doi.org/10.5281/zenodo.3332807)</figcaption>
</figure>

## Version control systems

Different version control systems can be used through a program with a graphical user interface, web browser-based applications, or command-line tools.Tools such as Google Drive and Dropbox offer platforms to update files and share them with others in real-time, collaboratively.

More sophisticated version control system exists within tools like [Google docs](https://docs.google.com/) or [HackMD](http://hackmd.io/).These allow collaborators to update files while storing each version in its version history (we will discuss this in detail).

Advanced version control systems (VCS) such as [Git](https://en.wikipedia.org/wiki/Git), [Mercurial](https://www.mercurial-scm.org/), and [SVN](https://subversion.apache.org/) provide much more powerful tools. Accessing the version history and keeping control over the main version of your files are particular feature of these advanced tools.

Versioning practices mainly come from managing changes in the code repositories. However, in reality, you can use version control for nearly any type of file on a computer.

### Motivation

In terms of reproducibility, version control is promordial in order to follow **provenance information**. Because data and analysis code do evolve over time, it can become very difficult or even impossible to know what version of the code and what version of the data was used to produce a particular figure. This provenance information is enabled and facilitated when both the data, the code and the figure files are under versioning.

In addition, version control creates **version history** to help us understand what changes were made, or why a specific analysis was run, even weeks or months later. With the help of comments and commit messages in Git, for instance, each version can explain what changes it contains compared to the previous versions. This is helpful when we share our analysis (not only data), and make it auditable or **reproducible** - which is good scientific practice.

A version control system **neatly hide older versions** of the data.  So your working directory is not cluttered by the debris of previous versions, while they remain accessible, in case you need them. Similarly, with version control, there is no need to leave unused chunks of code should you ever need to come back to an old version again.

Finally, version control is invaluable for collaborative projects where different people work on the same data or code simultaneously and build on each other's work.
Using a version control system, **changes made by different people can be tracked and often automatically combined**, saving a great deal of painstaking manual efforts. Using version control for your research project means that your work is more transparent. Because all your actions are recorded, your studies are easier to reproduce and build upon. Moreover, version control hosting services such as GitHub, GitLab and others provide a way to communicate and collaborate in a more structured way, such as in `pull requests`, `code reviews`, and `issues`.

### Potential

Here is a non-exhaustive list of features that a Git/GitHub workflow bring to data science projects, and that would be useful for research projects:

- Backup data by pushing the data to a Git platform, toward a public or private repository.
- Easily use different computers to work on the same project (with yourself of with collaborators).
- Keep track of contributions.
- Facilitate the use of folder templates to help with files organization.
- Use Git platforms tools for project management.
- Use Git platforms for outreach, even when the repository is private (using the Wiki).
- Create an associated website under the same organization on the Git platform.

I encourage you to use a Git platform that is provided as an open infrastructure. In many university, you will have access to a GitLab platform (which works very similarly to GitHub). 

### Limitations of Git

Git does not work well when there are a lot of data, or when the data are large. When you expect the project to get large, one needs to set a different tooling to avoid creating unpractical repositories. Some of these tools makes it more difficult to access or see you files, so it is important to plan in advance what tool will best suits your need.

**Briefly, in order to use Git when there are lots or large files, one needs to split the data in different repositories, and have these repositories use the git-annex technology.**

## Versioning Data 

Git is made for small files and stems from software development where most of the files are code files. If you have many or large (and binary) files (such as huge data tables, images etc.), you will need to use the Git submodules and git-annex technologies. Version controlling the components of evolving projects could help to make work more organised, efficient, collaborative, and reproducible. Many scientific projects, however, do not only contain code, manuscripts, or other small-sized files, but contain larger files such as large datasets, analysis results, or binary files (presentations, manuscripts, pdfs) which can change or be updated in a project just like other small sized text components.
In this chapter, we discuss why and how to do data versioning, especially why Git is not well suited for data versioning and what we can be done about it.

### Importance of Version Controlling Data

We should not hold the notion that the data used for analysis is static; once it is acquired, it does not change and serves as input for a given analysis and the backbone of our scientific results. The reality is that data is only rarely invariant. For example, throughout a scientific project, datasets can be extended with new data, adapted to new naming schemes, reorganized into different file hierarchies, updated with new data points or modified to fix any errors. Sometimes you might also want to experiment off different versions of the same dataset.

Such dynamic processes are excellent and beneficial for science as they ensure that data is usable and up-to-date, but they can be confusing if they are not
adequately documented. If a dataset that is the basis for computing a scientific result changes without version control, reproducibility can be threatened: results may become invalid, or scripts that are based on file names that change between versions can break. Especially if original data gets replaced with new data without version control in place, the original results of the analysis may not be reproduced. Therefore, version controlling data and other large files in a similar way to version controlling code or manuscripts can help ensure the reproducibility of a project and capture the provenance of results; that is "the precise subset and version of data a set of result originates from". Together with all other components of a research project, data identified in precise versions is part of the research outcome. The reproducibility aspect of a scientific project can improve a lot if we can track the subset or version of data a certain analysis or result is based upon.

<figure markdown="span">
  ![Project History](assets/images/Provenance.jpg){ width="600" }
  <figcaption>Provenance on which data in which version was underlying which computation is crucial for reproducibility. The Turing Way project illustration by Scriberia. Used under a CC-BY 4.0 licence. DOI: 10.5281/zenodo.3332807.</figcaption>
</figure>

### Challenges in Version Controlling Data

As we described earlier, there are limitations to Git. If others try to clone your repository or fetch/pull to update it locally, it will take longer to do this if it contains larger files that have been versioned and modified.

Accordingly, repository hosting services usually impose maximum file sizes on users. For example, if a single file in your repository exceeds 100MB, you will not be able to push this file to a GitHub repository. Furthermore, if a large file was accidentally added to a repository, removing the file from the repository can be tedious, as this file needs to be [purged](https://help.github.com/en/github/authenticating-to-github/removing-sensitive-data-from-a-repository).

### Tools for Version Controlling Data

Several tools are available to handle version controlling and sharing large files. Most of them integrate very well with Git and extend a repository's capabilities to version control large files. With these tools, large data can be added to a repository, version controlled, reverted to previous states, or updated and modified collaboratively, and even shared via GitHub as small-sized files.
Some of these tools include:

#### DVC

DVC (open-source Version Control System for Machine Learning Projects) https://dvc.org/.
DVC guarantees reproducibility by consistently maintaining a combination of input data, configuration, and the code that was initially used to run an experiment.

#### Git LFS

[Git LFS](https://git-lfs.github.com/) comes with a command-line extension to Git and allows you to treat files of any size alike, using standard Git commands. A major shortcoming, however, is that Git LFS is a _centralised_ solution. Large files are not distributed but stored on a remote server. This usually requires setting up your server or paying for a service - which can make it very inaccessible.

#### `git-annex`

The [`git-annex`](https://git-annex.branchable.com/) tool is a distributed system that can manage and share large files independent from a central service or server.
`git-annex` manages all file _content_ in a separate directory in the repository (`.git/annex/objects`, the so-called _annex_) and only places file _names_ with some metadata into version control by Git.
When a Git repository with an annex is pushed to a web-hosting service such as GitHub, the contents stored in the annex are not uploaded.
Instead, they can be pushed to a storage system (such as a web server, but also third party services such as Dropbox, Google Drive, Amazon S3, box.com, and [many more](https://git-annex.branchable.com/special_remotes/)).
If a repository with an annex is cloned, the clone will not contain the _contents_ of all annexed files by default, but display only file names.
This makes the repository small, even if it tracks hundreds of gigabytes of data, and cloning fast, while file contents are stored in one or more free or commercial external storage solutions.
On-demand, any file content can then be obtained with a `git-annex get` command from the external file storage.

#### git submodules

Submodules allows to split the data in different repositories, while keeping everything under a single "parent" repository.
It is very powerful, but difficult to use. Especially, using branches in  submodules make it complex to handle. However, this is the only tool listed here allowing to work with many files in a Git repository.

#### DataLad

[DataLad](https://www.datalad.org/), builds upon git and git-annex. Like `git-annex`, it allows you to version control data and share it via third-party providers but simplifies and extends this functionality. In addition to sharing and version controlling large files; it allows recording, sharing, and using software environments, recording and re-executing commands or data analyses, and operating seamlessly across a hierarchy of repositories. You can record in hte provenance history *where* you got the data from, *when* you run *which analysis* on the data and where you stored the *output* by using a single command additionally to all the code-version control advantages of git. 

**Please note:** Powerful version control systems such as Git or even more DataLad take time to learn. There are a lot of tutorials, especially for learning Git, however, you will only get the gist if you simply start using it and also make some mistake on the way. But don't worry, if you make a mistake with version control systems it won't destroy your project or make you loose data. 

**Another note:** When you use version control systems, you need to make sure what you include in the version control and how you control access and sharing. 


!!! info
    Most of the content was copied from [The Turing Way Handbook](https://the-turing-way.netlify.app/reproducible-research/vcs#) under a CC-BY 4.0 licence.

## optional/reading/further materials

#### Git 

- YouTube is full of Git/GitLab/GitHub videos for all kinds of levels and features!!! For example: Brainhack [Git introduction](https://youtu.be/fBgxmpk9C4I?si=im33MV2V0PV8uM0k) or [GitHub CI](https://youtu.be/VibDC49ZAJE?si=587WHWe1nZQzHIay)
- Git cheat sheet by [gitlab](https://about.gitlab.com/images/press/git-cheat-sheet.pdf) or [github](https://education.github.com/git-cheat-sheet-education.pdf)
- [Atlassian tutorials](https://www.atlassian.com/git/tutorials) and [cheat sheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)
- Troubleshooting: [Oh shit git](https://ohshitgit.com/) or [Dangit git](https://dangitgit.com/) (are the same, but the latter is without swearing)
- [Git branching](https://learngitbranching.js.org/?locale=de_DE)
- [Git GUIs](https://git-scm.com/downloads/guis) 
- [Advanced Git commands](https://www.atlassian.com/git/tutorials/advanced-overview)
- really, just type anything you want to know about Git in YouTube and you'll find a tutorial for it. I promise. 

#### DataLad 

- [DataLad Website](datalad.org)
- [DataLad Handbook](handbook.datalad.org)
- [DataLad@NeuroStars](neurostars.org/tag/datalad)
- [DataLad@YouTube](www.youtube.com/@DataLad)