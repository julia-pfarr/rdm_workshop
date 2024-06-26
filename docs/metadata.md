
!!! abstract "Objectives📍"

    - general Metadata (bibliographic/administrative Metadata)
    - content and field specific Metadata 


## Metadata = data about data

We all know and use metadata every day. See for yourself in this short video which kind of metadata you already know:

<p align="center"><iframe width="560" height="315" src="https://www.youtube.com/embed/3sLKVYYOM40?si=L7zxwPQ_IUdI68Vg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></p>

To get a sense of what Metadata for a research project should be you can simply ask yourself: "What would someone unfamiliar with your data (and possibly your research) need in order to find, evaluate, understand, and reuse them?

!!! note "Task" 
    Let's imagine someone gives you a value of their data which only says "Temperature 31.5". What questions would you ask this researcher in order to find out what "Temperature 31.5" means and be able to reuse it or make a decision about if you can reuse it for your own research?

??? tip "Possible questions"

    Temperature 31.5...

    - of what?
    - location?
    - in what unit?
    - is this value averaged?
    - collected how?
    - collected when?
    - precision/accuracy?
    - according to whom?
    - has anyone checked the quality of this value?

## General metadata for a research project

Having data available is of no use if it cannot be understood. Without metadata to provide provenance and context, the data can't be used effectively.
For example, a table of numbers is useless if no headings describe what the columns/rows contain.
Therefore you should ensure that open datasets include consistent metadata, that is information about the data so that the data is fully described.
This requires that information accompanying data is captured in documentation and metadata. 

**Documentation** provides context for your work. 
It allows your collaborators, colleagues and future you to understand what has been done and why.

Data documentation can be done on different levels. 
All documentation accompanying data should be written in clear, plain language. 
Documentation allows data users have sufficient information to understand the source, strengths, weaknesses, and analytical limitations of the data so that they can make informed decisions when using it. 

**Metadata** is information about the data, descriptors that facilitate cataloguing data and data discovery. 
Often, metadata are intended for *machine reading* while documentation is mostly written for *human reading*.

When data is submitted to a trusted data repository, the machine-readable metadata is generated by the repository. 
If the data is not in a repository a text file with machine-readable metadata can be added as part of the documentation.

- The type of research and the nature of the data also influence what kind of documentation is necessary. 
- The level of documentation and metadata will vary according to the project, and the range of people the data needs to be understood by.
- Examples of documentation may include items like [data dictionaries](https://help.osf.io/hc/en-us/articles/360019739054-How-to-Make-a-Data-Dictionary) (see [here for a template](https://data.nal.usda.gov/data-dictionary-blank-template)) or codebooks, protocols, logbooks or lab journals, README files, research logs, analysis syntax, algorithms and code comments.  
- Variables should be defined and explained using data dictionaries or codebooks.
- Data should be stored in logical and hierarchical folder structures, with a README file used to describe the structure.
The README file is helpful for others and will also help you find your data in the future.
See the [README template from Cornell](https://cornell.app.box.com/v/ReadmeTemplate) for an example.
- It is best practice to use recognized community metadata standards to make it easier for datasets to be combined.

**Example README content:**

- Short description of the study, motivation and background
- A description of the folder structure
- Time and location of data collection for the studies reported
- Software required to open or run any of the shared files
- Under which license(s) the files are shared: instructions for citing the project
- Information on the publication status of the studies
- Contact information for the authors: who the team members are and contact details of the project leads
- A list of all the shared files

## Tagging

Tags are keywords assigned to files, and a way to add metadata to a file to organise them more flexibly.
While a file can only be in one folder at a time, it can have an unlimited number of tags. 

Some tips include:

- Use short tag names (one or two words)
- Be consistent with tags
- Not all file formats allow tags, and when files are transferred tags may be stripped

See [Tagging and Finding Your Files by MIT libraries](https://libguides.mit.edu/metadataTools) for more information. 

!!! note "Task" 
    Go to your OSF project and insert the general Metadata. Give your project some tags.

!!! note "Task" 
    Make a README.md file for your project and with the content described in the README example above. 

## Community Standards - Metadata

The use of community-defined standards for metadata is vital for reproducible research and allows for the comparison of heterogeneous data from multiple sources, domains and disciplines.
Metadata standards are also discipline-specific.
Not every discipline may use metadata standards, however.
For the field of psychology and neuroscience, [BIDS](https://bids-standard.github.io/bids-starter-kit/folders_and_files/folders.html) defines for the different data modalities which metadata has to be available in the dataset, how it is supposed to be named and in which folder it has to be placed. 

Again, for the field of psychology and neuroscience, [BIDS](https://bids-standard.github.io/bids-starter-kit/folders_and_files/folders.html) defines for the different data modalities which metadata has to be available in the dataset, how it is supposed to be named and in which folder it has to be placed. 

There are also situations when researchers make use of more general metadata standards, for example when they use a generic archive to store their data they have to adhere to the metadata standards of the archive. In this case, a text file with discipline specific metadata can be added as part of the documentation. For this, you can also use the [DataCite generator](https://dhvlab.gwi.uni-muenchen.de/datacite-generator/) by the DataCite Metadata Working Group. [^1] [^2]

!!! note "Task"
    Go to the [DataCite generator](https://dhvlab.gwi.uni-muenchen.de/datacite-generator/) and generate a metadata file for your project.

## optional/reading/further materials

- [Full BIDS documentation](https://bids-specification.readthedocs.io/en/stable/)
- [BIDS Starter Kit Tutorials](https://bids-standard.github.io/bids-starter-kit/tutorials/tutorials.html)
- [BIDS Talks](osf.io/yn93h) where the background and philosophy of BIDS are explained 
- [BIDS cookbook](https://remi-gau.github.io/bids_cookbook/)
- [BIDS converters](https://bids.neuroimaging.io/benefits.html#converters)
- [BIDS validator](https://bids-standard.github.io/bids-validator/): checks if your dataset is in a valid BIDS format
- [BIDS Apps](https://bids-apps.neuroimaging.io/)
- You are very welcome to reach out to me if you want to start using BIDS. I know it's a lot and can be overwhelming in the beginning. I'm happy to help you get started!

!!! info
    Most of the content was copied from [The Turing Way Handbook](https://the-turing-way.netlify.app/reproducible-research/rdm/rdm-metadata) under a CC-BY 4.0 licence.

[^1]: DataCite Metadata Working Group. (2021). DataCite Metadata Schema Documentation for the Publication and Citation of Research Data and Other Research Outputs. Version 4.4. DataCite e.V. https://doi.org/10.14454/3w3z-sa82
[^2]: Bayer, Christiane, Frech, Andreas, Gabriel, Vanessa, Kümmet, Sonja, Lücke, Stephan, Munke, Johannes, Putnings, Markus, Rohrwild, Jürgen, Schulz, Julian, Spenger, Martin, & Weber, Tobias. (2022). DataCite Best Practice Guide (Version 2.0). Zenodo. https://doi.org/10.5281/zenodo.7040047
