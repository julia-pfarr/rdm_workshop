
!!! note "Objectives📍"

    - different data repositories
    - what to consider when sharing data

## Where to Store Data

- Most institutions will provide a _network drive_ that you can use to store data.
- _Portable storage media_ such as memory sticks (USB sticks) are more risky and vulnerable to loss and damage.
- _Cloud storage_ provides a convenient way to store, backup and retrieve data.
You should check terms of use before using them for your research data.

Especially if you are handling personal or sensitive data, you need to ensure the cloud option is compliant with any data protection rules the data is bound by.
To add an extra layer of security, you should encrypt devices and files where needed.

Your institution might provide local storage solutions and policies or guidelines restricting what you can use. Thus, we recommend you familiarise yourself with your local policies and recommendations. 

## Backups

To avoid losing your data, you should follow good backup practices.

- You should have 2 or 3 copies of your files, stored on
- at least 2 different storage media,
- in different locations.

Backups are ideally done automatically and should take into consideration your institute's guidelines. The more important the data and the more often the datasets change, the more frequently you should back them up. If your files take up a large amount of space and backing up all of them proves to be challenging or expensive, you may want to create a set of criteria for when you back up the data. This can be part of your RDMP.

Watch this video on [Safe data storage and backup](https://www.youtube.com/watch?v=bgbbToXHgW0) from the [TU Delft Open Science MOOC](https://online-learning.tudelft.nl/courses/open-science-sharing-your-research-with-the-world/).

## Data Repositories

When you are ready to release the data to the wider community, you can also search for the appropriate databases and repositories in [FAIRsharing](https://fairsharing.org/databases), according to your data type, and type of access to the data.

A repository is a place where digital objects can be stored and shared with others (see also [this repository definition](https://the-turing-way.netlify.app/afterword/glossary.html#term-Repository)).

Data repositories provide access to academic outputs that are reliably accessible to any web user (see the [OpenDOAR inclusion criteria](https://v2.sherpa.ac.uk/opendoar/about.html)). 
Repositories must earn the trust of the communities they intend to serve and demonstrate that they are reliable and capable of appropriately managing the data they hold ([Lin et al. (2020)](doi:10.1038/s41597-020-0486-7.)).

Long-term archiving repositories are designed for secure and permanent storage of data, ensuring data preservation over extended periods.
This differs from platforms like GitHub and GitLab which primarily serve as collaborative development tools, facilitating version control and project management in a more dynamic and transient environment.
Platforms such as GitHub and GitLab do not assign persistent identifiers to repositories, and their preservation policies are more flexible compared to those of data repositories. 

#### Repositories and FAIR

Selecting an appropriate repository for your research outputs has many benefits:

- It helps make your Research Objects more FAIR. This is achieved through:
    - Repositories assign a Persistent Identifier to your Research Objects, which makes them findable and citable. The most commonly used persistent identifiers for research objects is the Digital Object Identifier, usually abbreviated to DOI.
    - Repositories use metadata standards in describing your Research Object, which ensures that other people can find it using search engines.
    - Repositories add a licence to the Research Objects. A license describes to potential reusers of your work what they are allowed to do with it. 
    - Repositories provide documentation for Research Objects. This can be in the form of READMEs and/or wikis that provide a description of your project and why it might be relevant to people.
    - Encouraging widely-used file formats. Many repositories have restrictions on the file formats used to ensure the sustainability of Research Objects. Some file formats (especially proprietary ones with a limited user base) can become deprecated.

- It allows to determine the levels of access to Research Objects. There are good reasons to not to make all Research Objects completely open.
However, it's still worthwhile to at least open the metadata and provide an option for people to obtain access to the actual Research Objects if they have certain credentials or if they have been given explicit access. That way, your work will still be FAIR (because the metadata are findable and there is an access procedure in place), as well as and secure (because you can control who has access). Restricting access and storing data on European servers can help to manage sensitive data.

#### Selecting an appropriate repository

Data should be submitted to domain or discipline specific, community recognized, repository where possible. A general purpose repository can be used when there are no suitable discipline specific repositories. Discipline specific data repositories are likely to have more functionalities for the type of data that you would like to share, as well as community standards that you can adhere to to make the data more FAIR. 

The choice of repository can depend on multiple factors:

- Your discipline
- Type of digital output
- File size
- Policies/requirements from institutions, national policies, funding agencies
- Access restrictions

You can search for relevant repositories on [re3data](https://www.re3data.org/) and [FAIRsharing](https://fairsharing.org/). However, a search will likely result in a long list of repositories, which you will need to narrow down. The following questions may help you with that:

- Is the data repository discipline-specific and community-recognized? Does it use the recognized standards in my discipline?
- Is the data repository known by the research community?
- Are others using the data repository to share their data?
- Has a data repository been specified by my funder/publisher/institution?
- What are the file size requirements and limitations?
- What are the costs for data sharing?
- What data formats are allowed? Will it take the data that you want to share?
- Does it provide a persistent identifier, for example a Digital Object Identifier (DOI)?
- Does it provide the right type of access control that suits the sharing conditions of the data? (restricted access/embargo's)
- Is there support available on how to curate the data/metadata?

See the [ARDC's Guide to choosing a data repository](https://ardc.edu.au/resource/guide-to-choosing-a-data-repository) or the [DCC checklist for evaluating data repositories](https://www.dcc.ac.uk/guidance/how-guides/where-keep-research-data) for more information. 

Your institution might also provide you with a data repository. 

??? tip "General repositories"

    If your disicpline does not have a disciplinary specific repository you can make use of several general repositories. 
    Below follows a (non-exhaustive) list of these different types of repositories: 

    #### General purpose repositories

    - [Zenodo](https://zenodo.org/)
    - [Figshare](https://figshare.com/)

    #### Project repositories

    - [Open Science Framework (OSF)](https://osf.io/)
    - [Research Equals](https://www.researchequals.com/)
    - [Octopus](https://www.octopus.ac/)
    - [CRAN](https://cran.r-project.org/) for R-Packages

    #### Generic data repositories

    - [Dryad](https://datadryad.org/stash)
    - [Dataverse](https://dataverse.org/)
    - [4TU.ResearchData](https://data.4tu.nl/)
    - [UK Data Service](https://ukdataservice.ac.uk/)

## Data Sharing

### Motivations For Sharing Data

There are many reasons to share your research data publicly.

1. To allow the possibility to fully reproduce a scientific study.
2. To prevent duplicate efforts and speed up scientific progress.
Large amounts of research funds and careers of researchers can be wasted by only sharing a small part of research in the form of publications.
3. To facilitate collaboration and increase the impact and quality of scientific research.
4. To make results of research openly available as a public good, since research is often publicly funded.

??? tip "Steps To Share Your Data"

    **Step 1: Select what data you want to share**

    Not all data can be made openly available, due to ethical and commercial concerns, and you may decide that some of your intermediate data is too large to share. As such, you first need to decide which data you need to share for others to be able to reproduce your research.

    **Step 2: Choose a data repository or other sharing platform**

    Data should be shared in a formal, open, and indexed data repository where possible so that it will be accessible in the long run.
    Suitable data repositories by subject, content type or location can be found at [Re3data.org](https://www.re3data.org/), and in [FAIRsharing](https://fairsharing.org/databases) where you can also see which standards (metadata and identifier) the repositories implement and which journal/publisher recommend them. If possible use a repository that assigns a DOI, a digital object identifier, to make it easier for others to cite your data. 
    
    A few public data repositories are [Zenodo](https://zenodo.org/), [Figshare](https://figshare.com/), [Harvard Dataverse](https://dataverse.harvard.edu/), [4TU.ResearchData](https://data.4tu.nl/info/en), and [Dryad](https://datadryad.org/). 
    See the [NIH list of Generalist Repositories](https://sharing.nih.gov/data-management-and-sharing-policy/sharing-scientific-data/generalist-repositories) for more data repositories.

    **Step 3: Choose a licence and link to your paper and code**

    So that others know what they can do with your data, you need to apply a licence to your data.
    The most commonly used licences are [Creative Commons](https://creativecommons.org/choose/), [Open Government Licence](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/), or an [Open Data Commons Attribution License](https://opendatacommons.org/licenses/by/index.html).
    To get maximum value from data sharing, make sure that your paper and code both link to your data, and vice versa, to allow others understand your project better.

    **Step 4: Upload your data and documentation**

    In line with the FAIR-principles, upload the data in open formats as much as possible and include sufficient documentation and metadata so that someone else can understand your data.
    It is also essential to think about the file formats in which the information is provided.
    Data should be presented in structured and standardized formats to support interoperability, traceability, and effective reuse.
    In many cases, this will include providing data in multiple, standardized formats, so that it can be processed by computers and used by people.


#### Data Availability Statement

Once you made your data available, it is important to ensure that people can find it when they read the associated article.
You should cite your dataset directly in the paper in places where it is relevant, and include a citation in your reference list, as well as include a Data Availability Statement at the end of the paper (similar to the acknowledgement section).

#### Privacy And Data Protection

Many fields of research involve working with sensitive personal data, with medical research being the most obvious example. There are a number of strategies that you can adopt to **safeguard the privacy** of your research subjects:

**1. Data minimisation**

- If personal information isn't needed, don't collect it.
- Periodically review whether you are retaining unnecessary identifying information.
- When identifying information is no longer needed, safely remove, delete or destroy it.

**2. Data retention limits**

- Decide how long you will retain identifiable data before removing direct identifiers, applying more complex anonymisation techniques, or deleting the data altogether.
- When deleting sensitive data you need to be aware that standard methods for deleting files (for example moving files to the recycle bin and emptying it) are not secure. These deleted files may be recovered.  Use **software** like BleachBit (Linux, Windows), BC Wipe, DeleteOnClick and Eraser (Windows) or Permanent Eraser or 'secure empty trash' (Mac) to safely delete the data. An alternative is the **physical destruction** of the storage media. **Degaussing** disturbs the magnetic alignment of magnetic storage media (such as hard drives and tapes) and may render those unusable.  If you encrypted the data (see point 4 below), you can also **delete the encryption key**.

**3. Secure data transfer**

- Before deciding to transfer personal data, you should consider whether the transfer of identifiable data is necessary.
For example, can data be de-identified or anonymised? 
- If data cannot be made unidentifiable then you must ensure you have authority to transfer the personal data, and that there are appropriate safeguards in place to protect the data before, during and after transit.
- Keeping data in one place is safer than transfering it elsewhere. 
Consider whether it is possible to provide access to the data, instead of transferring them outside of your institution.
- Often your university or institute will provide solutions for secure file transfer. 
Contact you research data, privacy or IT support team for guidance. 

**4. Encryption** 

- Encryption provides protection by ensuring that only someone with the relevant encryption key (or password) will be able to access the contents.
    - Protect on disk level: Bitlocker for Windows, FileVault for MacOS
    - Protect on “container” level (a folder containing multiple files):  Veracrypt (or Archive for MacOS)
    - Portable storage: Bitlocker
    - File level / Exchange information:
      - Simple method: use 7zip, and pack with a password
      - More complicated to setup: use PGP tooling (can also be used to securely send email)
    - See the [Ghent University Encryption for Researchers manual](https://osf.io/nx8km/) for more details and step-by-step guides

**5. Access permissions**

- Control who has access to which parts of the data, and which type of permissions they have, such as "read" vs. "write" access.
- Deny access to sensitive data if that access is no longer needed.
- Password protection.


**6. Anonymization**

Anonymization is a process by which identifying information in a dataset is removed.  It is used primarily to allow data to be shared or published without revealing the confidential information it contains.

- Where possible, direct identifiers (such as names, addresses, telephone numbers and account numbers) should be removed as soon as the identifying information is no longer needed. 
You can delete the data or replace it with pseudonyms. 
For qualitative data you should replace or generalise identifying characteristics when transcribing interviews.
- De-identified data that can be re-identified using a linkage file (for example, information linking data subjects to identifiable individuals) is known as pseudonymized data. NOTE: In this instance, the linkage file should be encrypted and stored securely and separately from the de-identified research data. Identification of individuals in pseudonymized or de-identified data may still be possible using combinations of indirect identifiers (such as age, education, employment, geographic area and medical conditions). Further, data and outputs containing small cell counts may be potentially disclosive, particularly where samples are drawn from small populations or include cases with extreme values or relatively rare characteristics.

For more information about anonymization:

- Watch [this webinar by Enrico Glerean](https://www.youtube.com/watch?v=ILXeA4fx3cI) 
- Watch a presentation on [Amnesia – Data Anonymisation Made Easy](https://www.youtube.com/watch?v=9wu_xGeYsQw) or a webinar on [Amnesia - a tool to make anonymisation easy](https://www.youtube.com/watch?v=9wu_xGeYsQw)
- Or read an [explanation by the Finnish social science data archive](https://www.fsd.tuni.fi/en/services/data-management-guidelines/anonymisation-and-identifiers/)
- [Anonymisation step-by-step](https://ukdataservice.ac.uk/learning-hub/research-data-management/anonymisation/anonymisation-step-by-step/)


??? tip "Citing Research Objects"

    You should cite research objects directly in the paper in places where it is relevant. This is a commonly practised way of citing publications and is valid for citing other research components like data and software. A citation includes the following information:

    - Author
    - Title
    - Year of publication
    - Publisher (for data, this is often the data repository where it is housed)
    - Version (if indicated)
    - Access information (a URL or DOI)

    A citation style is a specific arrangement, order and formatting of information necessary for a citation. For instance, the MLA style was developed by Modern Language Association (originally used in the humanities) and the APA style was developed by American Psychological Association (originally used in psychology and the social sciences).

    - MLA citation style uses the following format:
    `Author. "Title of the Source." Title of the Container, Other contributors, Version, Number, Publisher, Publication date, Location.`
    - APA citation style uses the following format:
    `Author. (Year). Title of data set (Version number). [Retrieved from] ***OR*** [DOI]`

    See [Scribbr Citation Styles Guide](https://www.scribbr.com/citing-sources/citation-styles/).
    See also [FORCE11 resource](https://www.force11.org/node/4771).


??? tip "Citing Data"

    When sharing a dataset, use the assigned DOI (from the data repository) and add this to your data availability statement at the end of the paper (similar to the acknowledgement section). It is important to also cite your dataset in the references themselves, as only the citations in the reference section will contribute to citation counts. Data citation is important because it facilitates access, transparency and potentially reproducibility, reuse, and credit for researchers. It also provides recognition and visibility for the repositories that share data.

    You can find examples of these statements in the publishers' (research data) author policies.

    **Data availability statement examples:**

    **Using the Digital Object Identifier (DOI):**
    “The data that support the findings of this study are openly available in [repository name] at http://doi.org/[doi].”

    **If no DOI is issued:**
    - “The data that support the findings of this study are openly available in [repository name] at [URL], reference number [reference number].”

    **When there is an embargo period you can reserve your DOI and still include a reference to the dataset in your paper:**
    - “The data that support the findings will be available in [repository name] at [URL / DOI] following a [6 month] embargo from the date of publication to allow for the commercialisation of research findings.”

    **When data cannot be made available:**
    - “Restrictions apply to the data that support the findings of this study.
    [Explain nature of restrictions, for example, if the data contains information that could compromise the privacy of research participants] Data are available upon reasonable request by contacting [name and contact details] and with permission of [third party name].”
    -  “The data that support the findings of this study are available upon request.
    Access conditions and procedures can be found at [URL to restricted access repository such as [EASY](https://easy.dans.knaw.nl/ui/home).]”

    **When code is shared:**
    - Data and code to reproduce the results shown in the paper can be obtained from The Turing Way (2023) at Zenodo ([https://zenodo.org/doi/10.5281/zenodo.3233853](https://zenodo.org/doi/10.5281/zenodo.3233853)) and GitHub ([https://github.com/the-turing-way/the-turing-way](https://github.com/the-turing-way/the-turing-way)). We used R version 4.2.2 (*use citation() to check the suggested citation*) and the following R packages: ggplot2 ([Wickham 2016](https://cran.r-project.org/web/packages/ggplot2/citation.html)), another example (*and citation added to the references!*). 

    **More Data Availability Statement examples:**

    You can find more examples on the [Manchester's Data Access Statements page](https://www.library.manchester.ac.uk/using-the-library/staff/research/research-data-management/sharing/data-access-statements/), the [Cambridge Data Availability Statement examples](https://www.cambridge.org/core/services/authors/open-data/data-availability-statements), the [AMS Data Availability Statement examples](https://www.ametsoc.org/index.cfm/ams/publications/author-information/formatting-and-manuscript-components/data-availability-statement-examples/), or [Nature's Tips for writing a dazzling Data Availability Statement](https://researchdata.springernature.com/posts/tips-for-writing-a-dazzling-das-data-availability-statement).

??? tip "Citing Software"

    A software citation has a lot of the same elements as a data citation, described above, and are described in more detail in the [Software Citation Principles](https://www.force11.org/software-citation-principles).
    When using others software, it is vital to cite and attribute it properly.
    See also [How to Cite R and R Packages](https://ropensci.org/blog/2021/11/16/how-to-cite-r-and-r-packages/) for more information.

    === "GitHub"
        To make your code citable, you can use the integration between [Zenodo](https://zenodo.org/) and GitHub.

        * Create a file to tell people how to cite your software. Use this [handy guide](https://citation-file-format.github.io/cff-initializer-javascript/) to format the file.
        * Link your GitHub account with a Zenodo account. This guide explains [how](https://guides.github.com/activities/citable-code/).
        * You can tell Zenodo what information or metadata you want to include with your software by converting your `CITATION.cff` file to `zenodo.json`.

            ```bash
            pip install cffconvert
            cffconvert --validate
            cffconvert --format zenodo --outfile .zenodo.json
            ```

        * Add `.zenodo.json` to your repository.
        * On Zenodo, flip the switch to the 'on' position for the GitHub repository you want to release.
        * On GitHub, click the *Create a new release* button.
        Zenodo should automatically be notified and should make a snapshot copy of the current state of your repository (just one branch, without any history), and should also assign a persistent identifier (DOI) to that snapshot.
        * Use the DOI in any citations of your software and tell any collaborators and users to do the same!

    === "GitLab"

        To make your code citable, through an automated publication of your Gitlab repository to [Zenodo](https://zenodo.org/):

        * Create a file to tell people how to cite your software. Use this [handy guide](https://citation-file-format.github.io/cff-initializer-javascript/) to format the file.
        * Convert your `CITATION.cff` file to `.zenodo.json`.
        This file tells Zenodo what information or metadata you want to include with your software.

            ```bash
            pip install cffconvert
            cffconvert --validate
            cffconvert --format zenodo --outfile .zenodo.json 
            ```

        * Add `.zenodo.json` to your repository.
        * Use the [gitlab2zenodo](https://gitlab.com/sbeniamine/gitlab2zenodo) package to publish a snapshot of your repository to your Zenodo instance.
        By following the installation and setup instructions of this package, you will get a workflow on your CI options that will take care of the publication to Zenodo.
        * Use the DOI in any citations of your software and tell any collaborators and users to do the same!

        
    If you don't have a Zenodo record for your software yet when you attempt to publish it for the first time, you may encounter an error due to the undefined `ID`. To address this issue, we recommend manually creating a record on Zenodo and updating the value of the CI variable `zenodo_record`. Detailed instructions for this process can be found in the [gitlab2zenodo](https://gitlab.com/sbeniamine/gitlab2zenodo) installation and setup instruction.

### Additional resources on data sharing

- '[How can you make research data accessible?](https://www.software.ac.uk/how-can-you-make-research-data-accessible)': a blog that contains five steps to make your data more accessible
- The European Commission's [data guidelines](https://open-research-europe.ec.europa.eu/for-authors/data-guidelines)
- Videos on [Data sharing and reuse](https://www.youtube.com/watch?v=4igGBCggU0Y) & [Data Preservation and Archiving](https://www.youtube.com/watch?v=J76yTp8XE-0) from the [TU Delft Open Science MOOC](https://online-learning.tudelft.nl/courses/open-science-sharing-your-research-with-the-world/).
- [Webinar: Why share your data?](https://www.ebi.ac.uk/training/online/courses/bringing-data-life-data-management-biomolecular-sciences/why-share-your-data/)
- [Webinar: Publishing and citing data in practice by Jez Cope](https://youtu.be/PpMOkTnBMlI)
- Coursera Videos from [Research Data Management and Sharing](https://www.coursera.org/learn/data-management) on the [Benefits of Sharing](https://www.coursera.org/lecture/data-management/benefits-of-sharing-IPZ0h), [Why Archive Data?](https://www.coursera.org/lecture/data-management/why-archive-data-lcQ2m), and [Why is Archiving Data Important?](https://www.coursera.org/lecture/data-management/why-is-archiving-data-important-04Gji)
- [Blog: Ask not what you can do for open data; ask what open data can do for you](http://blogs.nature.com/naturejobs/2017/06/19/ask-not-what-you-can-do-for-open-data-ask-what-open-data-can-do-for-you/)
- Forschungsdaten.info: Datenschutzrecht (Data protection law) 
- [Brainhack School Module: Open Data](https://school.brainhackmtl.org/modules/open_data/)

!!! info
    Most of the content was copied from [The Turing Way Handbook](https://the-turing-way.netlify.app/reproducible-research/rdm/rdm-repository) under a CC-BY 4.0 licence.
