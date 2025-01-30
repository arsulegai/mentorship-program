# Hyperledger Mentorship Program

*   [Program Description](#program-description)
    *   [Benefits for Mentees](#benefits-for-mentees)
    *   [Benefits for Hyperledger Community](#benefits-for-hyperledger-community)
*   [2024 Program Dates\*](#2024-program-dates)
*   [Mentee Stipend](#mentee-stipend)
*   [Additional Mentoring Resource](#additional-mentoring-resource)
*   [Questions?](#questions)

# Program Description

The Hyperledger Mentorship Program is aimed at creating a structured hands-on learning opportunity for new contributors who may otherwise lack the opportunity to gain exposure to or entry into the Hyperledger open source development community. It also provides a more defined path for Hyperledger to connect with the next generation of developers and researchers to inject more talent into its community. Each mentee will apply and be matched with a mentor or mentors who are active contributors in the Hyperledger community. Each mentee will work remotely from their location of choice. Regular evaluation and feedback will be provided. Mentees will have the opportunity to showcase their learnings and contributions through blogging, speaking at meetups or regional events, or travel to a global Hyperledger event to present their work in person and network with others in the broader community.

## Benefits for Mentees

*   Mentees gain exposure to and first-hand experience with real-world open source software development
    
*   Mentees get introduced to open source development infrastructure, tooling, and culture, and best practices.
    
*   Mentees have the opportunity to be guided by open source professionals to contribute code, documentation, or research to make a real impact on large scale open source projects.
*   Mentees have the hands-on opportunity to do work related to their academic and professional interests and to further the pursuit of those interests.
    
*   Mentees develop close working relationships with open source professionals and industry business leaders to expand their professional network.
    
*   Mentees have the opportunity to showcase their work and to raise their profile in the DLT space and open source development community.

## Benefits for Hyperledger Community

*   More source code, documentations, and research get produced and used for the benefit of all.
*   It helps address gaps in feature/code development, research, and documentation that exist in projects and the community. 
*   It helps create a pipeline to a more diverse, well-educated pool of developers, researchers, and other contributors.
    
*   It helps spread the word about Hyperledger and its related technologies at academic institutions and increase academia’s interest in the teaching and research of the DLT technologies.
    
*   It helps Hyperledger gain valuable insight into new contributor onboarding processes and continuously find ways to lower the barriers for entry.
    
*   It creates positive press for Hyperledger via testimonials, brand recognition, and peer-to-peer messaging, and other types of content. 
    

# 2024 Program Dates\* 

*   05 Feb 2024 - 15 Mar 2024 community members submitting mentorship project proposals 
    
*   18 Mar 2024 - 29 Mar 2024mentorship project proposal review by [Technical Oversight Committee](https://toc.hyperledger.org/)
    
*   04 Apr 2024 - 10 May 2024 mentee application period on [LFX Mentorship](https://mentorship.lfx.linuxfoundation.org/)
*   13 May 2024 - 24 May 2024 mentee application review and applicant interview
    
*   27 May 2024 - 31 May 2024 selected mentee notification and acceptance
    
*   03 Jun 2024 - 14 Jun 2024 1st two weeks of June  onboarding/orientation sessions
*   17 Jun 2024 - 29 Nov 2024 **mentee/mentor working period** (mentees are expected to commit 15-20 hours a week on a consistent basis during this time) 
*   22 Jul 2024\- 26 Jul 2024  1st quarter mentee evaluation
*   02 Sep 2024 - 06 Sep 2024 midterm mentee evaluation, and midterm stipend will be paid to eligible mentees if they are in good standing following the midterm evaluation
*   14 Oct 2024 - 18 Oct 2024 3rd quarter mentee evaluation
*   25 Nov 2024\- 29 Nov 2024  final mentee evaluation, and final stipend will be paid to eligible mentees if they are in good standing following the final evaluation and successful completion of deliverables as determined by the mentor and program staff

\* *The program dates are subject to change without advanced notice*.

# Mentee Stipend

Mentees may be eligible to receive a stipend. The total stipend amount will be calculated using [a tiered structure based on the country where the mentee resides when participating in the program](https://docs.linuxfoundation.org/lfx/mentorship/mentee-stipends). The stipend will be paid in two installments provided that regular interval evaluations show the mentee eligible to received a stipend is making satisfactory progress. The final installment will be paid upon successful project completion as evaluated by the mentor(s) and the program staff. 

# Additional Mentoring Resource

  

Hyperledger Collaborative Learning Program (CLP) is a pilot program to connect those interested in mentoring with those seeking guided open source contribution experience. It is an extension of the regular Hyperledger Mentorship Program to offer additional mentoring resources to expand the number of new contributors receiving mentoring and guidance to enter the community and to become a productive active contributor to the Hyperledger open source community. Please visit the [CLP](https://lf-hyperledger.atlassian.net/wiki/display/CLP/Collaborative+Learning+Program) page for additional details.  

# Questions?

Please email [mentorship@hyperledger.org](mailto:mentorship@hyperledger.org)





# Introduction

This repository contains a template that will allow you to quickly bring up a documentation site for Hyperledger _PROJECT_. In general, the template provides suggested topics that should be covered in your documentation; however, you can always add/remove content to fit the needs of the project.

The following changes need to be done to update the documentation for your project.

## Configuration Updates

### Site Name

Change the `site_name` tag in `mkdocs.yml` to reflect the name of your Hyperledger project.

!!! example
    ``` yaml
    site_name: Hyperledger Bevel
    ```

### Repo URL

Change the `repo_url` tag in `mkdocs.yml` to reflect the repository of your Hyperledger project.

!!! example
    ``` yaml
    repo_url: https://github.com/hyperledger/_PROJECT_
    ```

### Project Logo

Replace the file `docs/assets/project-logo.png` with the logo for your project.

!!! tip

    White logos with a transparent background works best for the project logo.

!!! warning Logo Filename

    If you use a different name than `project-logo.png`, you will also need to update the `mkdocs.yml` file to replace the `theme.logo` tag to reflect the correct filename. Example:

    !!! example
        ``` yaml
        theme:
          logo: assets/name-of-logo-file.png
        ```

### Project Icon

Replace the file `docs/assets/project-icon.png` with the icon for your project.

!!! tip

    Color or dark icons works best for the project icon.

!!! warning Icon Filename

    If you use a different name than `project-icon.png`, you will also need to update the `mkdocs.yml` file to replace the `theme.favicon` tag to reflect the correct filename. Example:

    !!! example
        ``` yaml
        theme:
          favicon: assets/name-of-icon-file.png
        ```

## Documentation Updates

### Overall

Find and replace the use of `_PROJECT_` with the name of your project in all markdown files and the `mkdocs.yml` file.

### Introduction

Update the `docs/index.md` file to provide an introduction to the project.

### Concepts

The `docs/concepts` directory will contain information about the relevant concepts for your project. Currently there are placeholders for three concepts (`docs/concepts/concepts-[123].md`). You can remove these files and add a separate markdown file for each of the relevant concepts. Then modify the `mkdocs.yml` `nav` section to reflect the concept name and pointer to the concept. The relevant portion of the `mkdocs.yml` file is:

!!! example
    ``` yaml
    nav:
     - Concepts:
       - Concept 1: concepts/concept-1.md
       - Concept 2: concepts/concept-2.md
       - Concept 3: concepts/concept-3.md
    ```

### Getting Started

The files in the Getting Started topic are intended to help people get up and running with your project. 

* Installation (`docs/getting-started/installation.md`) - provide details on how to install the project.
* Running (`docs/getting-started/running.md`) - provide details on how to run the project.

### Tutorials

The `docs/tutorials` directory will contain tutorials that the use can use to learn about your project. There is an introduction page that you can use to describe your tutorials at a high level. In addition, there are placeholders for three tutorials (`docs/tutorials/tutorials-[123].md`). You can remove the placeholder files and add a separate markdown file for each of the relevant tutorials. Then modify the `mkdocs.yml` `nav` section to reflect the tutorial name, and pointer to the tutorial. The relevant portion of the `mkdocs.yml` file is:

!!! example
    ``` yaml
    nav:
     - Tutorials:
       - Introduction: tutorials/index.md
       - Tutorial 1: tutorials/tutorial-1.md
       - Tutorial 2: tutorials/tutorial-2.md
       - Tutorial 3: tutorials/tutorial-3.md
    ```
### Guides

In the Guides section, there are three placeholders:
1. Operations (`docs/guides/operations.md`) - used to guide an operator of your project through critical tasks.
2. Developers (`docs/guides/developers.md`) - used to guide a developer using your project through critical tasks.
3. Upgrading (`docs/guides/upgrading.md`) - used to guide someone through upgrading from one version of your project to another.

!!! note
    The placeholders are not all inclusive. Please add any other reference material that is needed and update the `mkdocs.yml` `nav` section to ensure these references show up on the documentation site.

### References

In the References section, there are three placeholders:

1. Architecture (`docs/references/architecture.md`) - describe the architecture for the project in this file.
2. Commands (`docs/references/commands.md`) - describe the different commands that are available for running the project.
3. Roadmap (`docs/references/roadmap.md`) - describe the roadmap for the project.

!!! note
    The placeholders are not all inclusive. Please add any other reference material that is needed and update the `mkdocs.yml` `nav` section to ensure these references show up on the documentation site.

### Contributing

The files in the Contributing topic are intended to help people who are interested in contributing to your project.

!!! note
    Sample text has been provided in these files. Feel free to modify to fit your project.

* How to Contribute (`docs/contributing/how-to-contribute.md`) - provide details on how to contribute to the project.
* Reporting a Bug (`docs/contributing/reporting-a-bug.md`) - provide details on how to report a bug.
* Requesting a Change (`docs/contributing/requesting-a-change.md`) - provide details on how to request a change. 
* Asking a Question (`docs/contributing/asking-a-question.md`) - provide details on how and where to ask questions.

### FAQs

There is a placeholder (`docs/faqs.md`) for including any frequently asked questions about the project. Please update this document whenever you come across a frequently asked question.

### Glossary

There is a placeholder (`docs/glossary.md`) for capturing terms that are used in the documentation and with relation to the project. Please update the glossary to include relevant terms and definitions.
