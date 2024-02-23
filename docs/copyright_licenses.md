
'Intellectual Property (IP)' law is a complex subject. However some understanding of it is important for anyone producing creative works governed by it including software, datasets, graphics and more. This is true irrespective of the nature of your project: Closed commercial projects building on open tooling; Commercial projects maintaining an open resource; Open community driven and/or non-profit projects. Each of these may need to make slightly different licensing choices from the beginning of their projects to be compatible with their goals. Decisions about licencing made at the inception of a project can have long-lasting and significant ramifications. The choices that you make about how your work is licensed shape who can and cannot legally use your work and for what purpose.

Many of the concepts which apply to the licensing of software, data, AI/ML models, hardware and other creative works such as visuals share common attributes and concepts which will be covered here.

Intellectual property is an umbrella term that refers to a number of distinct areas of law, primarily these three:

- **[Copyright](https://europa.eu/youreurope/business/running-business/intellectual-property/copyright/index_en.htm#shortcut-1/)**
- **[Patent](https://www.wipo.int/patents/en/)** (not discussed here)
- **[Trademark](https://euipo.europa.eu/ohimportal/en/trade-mark-definition/)** (not discussed here)

What these have in common is the attempt to extend property rights to intangible goods, meaning their use by others can be prevented or [licensed](https://www.oshwa.org/faq/#what-is-a-license/). Governments with such laws effectively create a limited grant of monopoly over these goods for their creators, and other holders of these rights. This is generally done with the ostensible intent to incentivise the creation and improvement of such goods, but can in practice result in perverse incentives which fail to do so.

!!! info "Note"
    It is important to consider that copyright, licenses, and patents are all legal concepts. As such, they are subject to what the law prescribes, which may change over time and space. Simply put, different countries have different laws, and follow different procedures with regard to enforcing them. The content provided here is broadly based on American and European law and legal traditions. It might not be applicable - might even be contra indicated - or relevant in your particular context. However most nations are signatories to international treaty agreements which somewhat harmonise these laws notably the Berne Convention, the [TRIPS Agreement](https://www.wto.org/english/docs_e/legal_e/27-trips_01_e.htm), and others under the [World Intellectual Property Organization (WIPO)](https://www.wipo.int/portal/en/index.html). Whilst international efforts have sought to harmonize copyright enforcement, the real world is a messy place.

!!! info "Another note"

    Good legal advice is timely, specific, and given by an expert; this chapter is none of these. It was written by engineers & scientists, not by lawyers, and it is a heavily simplified overview of a very complex field. The intent is to give you an overview of the basics so that you will know when to check whether something you want to do has potential legal ramifications. Do not make any important decisions based solely on the contents of this chapter.

    So do not take the descriptions provided or viewpoints shared as legal advice, they are not that. This document is not intended to be used in that manner. Consult a legal expert to provide actual legal advice for your case.

## Copyright

(Research) Data per se are not protected by copyright. A copyright only applies to a “personal intellectual creation” (§ Abs. 2 UrhG) (=criterium individuality). This is not true for data, as data is seen as facts. This means for data, only the structure of it can be protected by copyright (§ 4 UrhG). For example: The initial table with the data is not protected by copyright, but if the researchers invested comprehensive re-structuring of the data (e.g., by adding new derivatives of the data after pre-processing), a copyright hold by the creator is valid. The same is true for metadata. Beholder of the copyright is always the creator, i.e., the researcher. If the dataset was created in collaboration, all collaborators share the same copyright.

Professors are not obligated to share the created datasets with the university as it is implied that the research work of professors are not bound by instructions of the university (“nicht weisungsgebunden”). It is different for students and other scientific staff as their work is usually bound to instructions of the university (“weisungsgebunden”). This means, that the university holds usage rights for datasets specifically created for theses (Bachelor, Master, Dissertation) by students. Third-party funders such as the DFG do not have any usage rights, but expect the researchers to take care of this by themselves. There are no regulations to which extend researchers should share their data but they highly recommend to share as much as possible.

By default, if you make a work publicly available, you retain the copyright to that work and all rights that this gives you over it. Anyone wishing to re-use that work must seek to license the right to do so from you, or open themselves to the possibility of a lawsuit for infringing on your copyright.

### optional/reading/further materials

- [Urheberrecht in der Wissenschaft (Copyright law in academia) (insb. 24ff)](https://www.bmbf.de/SharedDocs/Publikationen/de/bmbf/1/31518_Urheberrecht_in_der_Wissenschaft.pdf?__blob=publicationFile&amp;v=3)
- [Datenschutzrecht (Data protection law)](https://forschungsdaten.info/themen/rechte-und-pflichten/datenschutzrecht/)
- [Urheberrecht (Copyright law)](https://forschungsdaten.info/themen/rechte-und-pflichten/urheberrecht/)
- [Rechtsfragen bei Open Science (Legal Issues with Open Science)](https://nbn-resolving.org/urn/resolver.pl?urn:nbn:de:gbv:18-3-2112)
- [Wem "gehören" Forschungsdaten?](https://www.forschung-und-lehre.de/forschung/wem-gehoeren-forschungsdaten-1013/) 
- [Gutachten zu den rechtlichen Rahmenbedingungen des Forschungsdatenmanagements (Expert opinion on the legal framework of Research Data Management)](https://tu-dresden.de/gsw/phil/irget/jfbimd13/ressourcen/dateien/dateien/DataJus/DataJus_Zusammenfassung_Gutachten_12-07-18.pdf?lang=de)
- [Fact Sheet Personal Data](https://zenodo.org/record/4035992#.ZC2f4uxBxz8)
- [Asking for permission](https://copyright.columbia.edu/basics/permissions-and-licensing.html)
- [Ethics and data protection](https://ec.europa.eu/info/funding-tenders/opportunities/docs/2021-2027/horizon/guidance/ethics-and-data-protection_he_en.pdf)
- [Rechtliche Rahmenbedingungen des Forschungsdatenmanagements](https://zenodo.org/record/4625417#.ZC2f_-xBxz8)
- [Data Protection Decision Tree](https://ec.europa.eu/assets/rtd/ethics-data-protection-decision-tree/index.html)
- [FDM Recht](https://kups.ub.uni-koeln.de/45599/1/fdm-recht.pdf)

## Licenses

### What are 'Usage Restricting' Licenses?

Usage restricting licenses seek to affirmatively protect users or others affected by the use of the work by placing specific restrictions on its use.
This curtails freedom 0, the freedom to use software 'for any purpose' and prohibiting the use of the software, or other system, for unethical purposes.
Both 'Ethical source' & 'Responsible AI' Licenses are examples of this approach and seek to place restrictions on the uses to which the licensees can put the software or machine learning systems licensed in this fashion.
Consequently, these licenses by the classical definitions of free and open source software from the FSF and OSI would not be considered free or open source licenses. They do however generally resemble them in the other three criteria of the definition.
Their merits versus conventional open source licenses have been the subject of some debate, and their adoption has thus far been relatively limited.

Even an attribution requirement (the BY in CC-BY) can in some cases be considered a usage restriction.
For example the Debian project found the [Common Public Attribution License (CPAL)](https://en.wikipedia.org/wiki/Common_Public_Attribution_License) to be incompatible their free-software guidelines for this reason whilst it is approved by the Open Source Initiative.
In the case of academic works attribution requirements can serve to re-enforce the citation convention with the force of copyright law.

### Where to find open licenses for different types of work

- Code
    - The [Open Source Initiaitive (OSI)](https://opensource.org/licenses/) maintains a list of [approved licenses](https://opensource.org/licenses/) open source licenses
    - [Free Software Foundation](https://www.fsf.org/) maintains a [list of GPL-Compatible Free Software Licenses](https://www.gnu.org/licenses/license-list.html#SoftwareLicenses)
        - [GNU/FSF recomendations](https://www.gnu.org/licenses/license-recommendations.html)
    - [choosealicense.com](https://choosealicense.com/) provides a tool to guide you through the license choice project.
    - [Organisation for ethical source](https://ethicalsource.dev/) maintains a list of [ethical source licenses](https://ethicalsource.dev/licenses/)
- Prose, Images, Audio, Video, Datasets, and similar
    - [Creative Commons (CC)](https://creativecommons.org/)
        - [Creative Commons License Chooser](https://creativecommons.org/choose/)
- Machine Learning (ML) / artificial inteligence (AI) systems
    - Creative commons and Software licenses can be applied to different parts of ML/AI systems, CC to training data and weights, software licenses to code used in training / depoyment.
    - [Responsible AI Licenses (RAIL)](https://www.licenses.ai/)

### Licencing enforcement

There have been a number of successful legal cases that have been brought in defence of the terms of copyleft licenses obliging the parties abusing the terms of these licenses to appropriately release their code.
But this can be hard to discover, as it is not immediately obvious if copyleft code has been used from looking at a black box proprietary end product.

Organisations which take legal action in defence of free software, and which can provide information and resources for anyone else seeking to do the same, include:

- [Software Freedom concervancy](https://sfconservancy.org/)
- [Software Freedom Law Centre](https://softwarefreedom.org/)
- [FSF - licensing and compliance](https://www.fsf.org/licensing/)
- [Free Software Foundation Europe (FSFe) - legal work](https://fsfe.org/activities/legal.en.html)
- [Electronic Fontiers Foundation - legal cases](https://www.eff.org/cases)

#### Contributor license Agreements

The holder of the copyright on a copyleft project can still re-license that project or dual-license that project under a different license, for example to grant exclusive rights to commercially distribute that project with proprietary extensions or to make future versions proprietary.
In a large community developed project, this would require the consent of all contributors, as they each own the copyright to their contributions.
To get around this, some copyleft projects developed by companies that commercially license proprietary extensions to these projects ask their contributors to sign contributor license agreements (CLAs) which may assign the contributor's copyright to the company, or include other provisions so that they can legally dual-license the project.

#### How and where to add licenses

Wherever you share your project it is likely to be organised in a heirarchy of directories, place a plain text file containing the license in the top level directoty of your project.
If it is a git project for example that is shared on a git forge like github or gitlab, using a standard file name like `LICENSE` will allow your license to be picked up the the host and displayed on your project.
If the license that you have used has a standarised short name from [SPDX](https://spdx.org/licenses/) then this will be displayed as a small icon on your projects home page by these hosts.
It can also be useful to include license information in the form of standard strings at the top of each text file in your project.
There are useful tools which automate this available from [REUSE](https://reuse.software/) a project from the [FSFe](https://fsfe.org/) which developed the spec.
This is especially true if your project contains material that is licensed in multiple different ways or a part of your project is being used in someone else's which uses a different (compatible) license.

!!! note "Task"
    Got to your OSF project and add a LICENSE file. 
