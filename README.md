<!--
author:   Sibylle Vonesch, Ruben Vazquezuribe
email:    trainingandconferences@vib.be
version:  2.0.0
language: en
narrator: UK English Female

icon:     https://vib.be/sites/vib.sites.vib.be/files/logo_VIB_noTagline.svg

comment:  This document shall provide an entire compendium and course on the
          development of Open-courSes with [LiaScript](https://LiaScript.github.io).
          As the language and the systems grows, also this document will be updated.
          Feel free to fork or copy it, translations are very welcome...

script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js
          https://felixhao28.github.io/JSCPP/dist/JSCPP.es5.min.js

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css
link:     https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css
link:     https://raw.githubusercontent.com/vib-tcp/material-liascript/master/img/org.css
link:     https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.11.2/css/all.min.css
link:     https://fonts.googleapis.com/css2?family=Saira+Condensed:wght@300&display=swap
link:     https://fonts.googleapis.com/css2?family=Open+Sans&display=swap

link:  https://raw.githubusercontent.com/vib-tcp/material-liascript/master/vib-styles.css

@edition:  2nd 
@CourseTitle: CRISPR in action: practice and theory of genome engineering

import:   https://raw.githubusercontent.com/vib-tcp/training_material_template/refs/heads/main/macro.md

-->

# @CourseTitle

<section>

Hello and welcome to our workshop! We are very happy to have you here.

This is the @edition edition of this workshop.

> We are using the interactive Open Educational Resource online/offline course infrastructure called LiaScript.
> It is a distributed way of creating and sharing educational content hosted on github.
> To see this document as an interactive LiaScript rendered version, click on the
> following link/badge: [LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/vib-tcp/training_material_template/main/README.md)

## General context

CRISPR technology has revolutionized genome editing, making precise genetic modifications faster and more accessible than ever before. For researchers entering the field of molecular biology or genetics, understanding CRISPR is no longer optional; it's essential. 

This introductory course provides a solid foundation in both the theoretical principles and practical applications of CRISPR. Through interactive lectures and guided lab sessions, participants will learn how to design gRNAs, construct CRISPR vectors, perform genome editing, and analyze editing outcomes. 

By the end of the training, you will be equipped with the skills to plan and execute your own CRISPR-based experiments confidentially, bridging the gap between concept and practice. 

## Proposed Schedule 

**Day 1 (9h00 to 17h30):**

- Introduction & Course overview

- Introduction to CRISPR/Cas9

- Lab introduction

- gRNA design for NHEJ/ Whole-Gene Knockout (theory & practical)

- Lab sessions 1 - gRNA cloning

**Day 2 (9h00 to 17h30):**

- Lab session 2 - gRNA cloning (continued), donor generation

- DNA repair pathways; gRNA & donor design for HDR (theory & practical)

- Lab session 3 - donor generation (continued), prepare editing experiments

**Day 3 (9h00 to 16h30):**

- Lab session 4 - editing experiments

- Invited Speaker

**Day 4 (9h00 to 16h30):**

- Primer design for edit confirmation (theory + practical)

- Lab session 5 - evaluate editing via colony PCR & Sanger sequencing

- Invited Speaker

**Day 5 (9h00 to 16h00):**

- Analyzing genotyping results (theory + practical)

- Global analysis of editing efficacy (practical)

- Methods to enhance HDR in bacteria & eukaryotes

- Beyond CRISPR/Cas9

- Wrap-up

</section>

# Lesson overview

> <i class="fa fa-lock"></i> **License:** [Creative Commons Attribution 4.0 International  License](https://creativecommons.org/licenses/by/4.0/deed.en)
>
> <i class="fa fa-user"></i> **Target Audience:** Researchers, PhD students, Post-docs
>
> <svg xmlns="http://www.w3.org/2000/svg" height="14" width="16" viewBox="0 0 576 512"><!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2023 Fonticons, Inc.--><path d="M384 64c0-17.7 14.3-32 32-32H544c17.7 0 32 14.3 32 32s-14.3 32-32 32H448v96c0 17.7-14.3 32-32 32H320v96c0 17.7-14.3 32-32 32H192v96c0 17.7-14.3 32-32 32H32c-17.7 0-32-14.3-32-32s14.3-32 32-32h96V320c0-17.7 14.3-32 32-32h96V192c0-17.7 14.3-32 32-32h96V64z"/></svg> **Level:** Intermediary  
>
> <i class="fa fa-arrow-left"></i> **Prerequisites**  
> To be able to follow this course, learners should have knowledge in:
> 
> 1. In depth theoretical knowledge of Molecular Biology
> 2. Basic experience with molecular tecniques (PCR, eletrophoresis,etc)
>
> <i class="fa fa-bookmark"></i> **Description**  
> 
> - The course combines interactive lectures with practical lab sessions to provide a solid understanding of CRISPR technology and enable students to apply it effectively.
>
> - Participants actively engage in designing experiments, performing genome editing using provided kits, and analyzing results under the guidance of experienced trainers.
>
> - Participants are expected to participate in discussions, apply theoretical concepts to hands-on tasks, and collaborate with peers to troubleshoot and refine experimental strategies.
> 
> <i class="fa fa-arrow-right"></i> **Learning Outcomes:**
>  
> By the end of the course, learners will be able to:
>
>1. Design gRNAs applying principles of efficiency prediction and off-target risk assessment.
>
>2. Construct CRISPR vectors using appropriate cloning strategies and component selection. 
>
>3. Optimize HDR donor templates for precise genome edits based on design criteria. 
>
>4. Perform genome editing and genotyping analysis using Sanger sequencing and interpret editing efficacy 
>
>5. Learn about different approaches to analyzing CRISPR experiments and get experience in analyzing experimental data with varying bioinformatics tools. 
>
>6. Critique potential experimental pitfalls and propose improvements for CRISPR-based workflows.
>
> <i class="fa fa-hourglass"></i> **Time estimation**: 40h
>
> <i class="fa fa-asterisk"></i> **Requirements:** 
>
> Install and make account for:
> 
> - Benchling - gRNA and donor design, evaluation of editing outcomes
>
> - CRISPOR, CHOPCHOP - gRNA design
>
> - TIDE, CRISPResso2 - analyzing sequencing results
>
> <i class="fa fa-envelope-open-text"></i> **Supporting Materials**:
> 
> 1. [Slides](./docs/presentations/)  
> 
> <i class="fa fa-life-ring"></i> **Acknowledgement**:
>
> * [VIB Technologies](https://www.vib.be/)
>
> <i class="fa fa-money-bill"></i> **Funding:** 
>
> <i class="fa fa-anchor"></i> **PURL**:  


# Authors and Contributors

Authors

- @[orcid(Sibylle Vonesch)](http://orcid.org/0000-0003-2485-1048)
- @[orcid(Ruben Vazquezuribe)](http://orcid.org/0000-0002-9800-0409)


## Citing this lesson

Please cite as:

  1. to be updated soon

# Chapters List

| Chapter | Title                                                   |
| :---- | :------------------------------------------------         |
| 0     | [You need before the course](./docs/chapters/GetReady4training.md) |

# References

Here are some great tips for learning and to get inspired f:

- Resource ([link](https://www.nextflow.io/docs/latest/index.html))

# About us

*About ELIXIR Training Platform*

The ELIXIR Training Platform was established to develop a training community that spans all ELIXIR member states (see the list of Training Coordinators). It aims to strengthen national training programmes, grow bioinformatics training capacity and competence across Europe, and empower researchers to use ELIXIR's services and tools.

One service offered by the Training Platform is TeSS, the training registry for the ELIXIR community. Together with ELIXIR France and ELIXIR Slovenia, VIB as lead node for ELIXIR Belgium is engaged in consolidating quality and impact of the TeSS training resources (2022-23) (https://elixir-europe.org/internal-projects/commissioned-services/2022-trp3).

The Training eSupport System was developed to help trainees, trainers and their institutions to have a one-stop shop where they can share and find information about training and events, including training material. This way we can create a catalogue that can be shared within the community. How it works is what we are going to find out in this course.

*About VIB and VIB Technologies*

VIB is an entrepreneurial non-profit research institute, with a clear focus on groundbreaking strategic basic research in life sciences and operates in close partnership with the five universities in Flanders – Ghent University, KU Leuven, University of Antwerp, Vrije Universiteit Brussel and Hasselt University.

As part of the VIB Technologies, the 12 VIB Core Facilities, provide support in a wide array of research fields and housing specialized scientific equipment for each discipline. Science and technology go hand in hand. New technologies advance science and often accelerate breakthroughs in scientific research. VIB has a visionary approach to science and technology, founded on its ability to identify and foster new innovations in life sciences.

The goal of VIB Technology Training is to up-skill life scientists to excel in the domains of VIB Technologies, Bioinformatics & AI, Software Development, and Research Data Management.

--------------------------------------------

*Editorial team for this course*

Authors: @[orcid(Alexander Botzki)](https://orcid.org/0000-0001-6691-4233), @[orcid(Bruna Piereck)](https://orcid.org/0000-0001-5958-0669)

Technical Editors: Alexander Botzki

License: [![CC BY SA](img/picture003.jpg)](https://creativecommons.org/licenses/by-sa/4.0/deed.en)

```json   @JSONLD
{
  "@context": "https://schema.org/",
  "@type": "LearningResource",
  "@id": "https://github.dev/vib-training-conferences/CRISPR-practice_n_theory-genome-engineering",
  "http://purl.org/dc/terms/conformsTo": {
    "@type": "CreativeWork",
    "@id": "https://bioschemas.org/profiles/TrainingMaterial/1.0-RELEASE"
  },
  "description": "This introductory course provides a solid foundation in both the theoretical principles and practical applications of CRISPR. Through interactive lectures and guided lab sessions, participants will learn how to design gRNAs, construct CRISPR vectors, perform genome editing, and analyze editing outcomes. ",
  "keywords": "CRISPR, Genome editing, Wet lab",
  "name": "CRISPR in action: practice and theory of genome engineering",
  "license": "https://creativecommons.org/licenses/by/4.0/",
  "educationalLevel": "intermediary",
  "competencyRequired": "Molecular Biology theoretical knowledge",
  "teaches": [
    "Design gRNAs applying principles of efficiency prediction and off-target risk assessment.",
    "Construct CRISPR vectors using appropriate cloning strategies and component selection.",
    "Optimize HDR donor templates for precise genome edits based on design criteria.",
    "Perform genome editing and genotyping analysis using Sanger sequencing and interpret editing efficacy.",
    "Learn about different approaches to analyzing CRISPR experiments and get experience in analyzing experimental data with varying bioinformatics tools.",
    "Critique potential experimental pitfalls and propose improvements for CRISPR-based workflows."
  ],
  "audience": "researchers, PhD students, Post-docs",
  "inLanguage": "en-US",
  "learningResourceType": [
    "Presentations, slides"
  ],
  "author": [
    {
      "@type": "Person",
      "name": "Sibylle Vonesch"
    },
    {
      "@type": "Person",
      "name": "Ruben Vazquezuribe"
    },
  ],
  "contributor": [
    {
      "@type": "Person",
      "name": "name"
    },
    {
      "@type": "Person",
      "name": "name"
    },
    {
      "@type": "Person",
      "name": "name"
    }
  ]
}
```











