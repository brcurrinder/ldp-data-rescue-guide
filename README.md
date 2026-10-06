# The Living Data Project: Data Rescue Guidebook

This repository contains the source files for **The Living Data Project: Data Rescue Guidebook**, a Quarto book developed to support interns, graduate student teams, and others working on data rescue projects through the [Living Data Project](https://livingdata.ca/), an initiative of the Canadian Institute of Ecology and Evolution (CIEE).

The guidebook introduces practical approaches for recovering, documenting, cleaning, validating, and preparing legacy datasets for long-term preservation and reuse. Although many examples come from ecological and freshwater datasets, most of the principles and workflows are broadly applicable to other research data.

## Read the guidebook

The rendered guidebook is available online at:

<https://brcurrinder.github.io/ldp-data-rescue-guide/>

The online version is the easiest way to work through the guidebook and includes navigation, searchable content, code examples, downloadable templates, and links to additional resources.

## What the guidebook covers

The guidebook is designed to help readers:

- Assess legacy datasets and associated documentation
- Reconstruct and improve dataset-level and observation-level metadata
- Understand data structure, tidy data, and relationships among tables
- Use reproducible workflows for data cleaning and validation
- Document decisions, assumptions, and unresolved issues
- Work collaboratively with data owners and data stewards
- Prepare data and metadata for long-term archiving and publication
- Understand FAIR, CARE, and related principles of responsible data stewardship
- Prepare ecological datasets for publication on data repositories
- Prepare freshwater monitoring datasets for publication on DataStream
- Use R, Git, GitHub, and other tools to support reproducible data rescue

The guidebook is intended to function both as a **learning resource** and as a **reference that teams can return to throughout a data rescue project**.

## Guidebook organization

The guidebook includes chapters on:

- Foundations of data rescue
- Data and metadata principles
- Repositories, persistent identifiers, and data publication
- Open science and reproducible research
- Collaboration and reproducible coding practices
- A general data rescue workflow
- DataStream-specific data rescue workflows
- Worked examples and case studies

Not every project will require every step described in the guidebook. Data rescue is often iterative, and the appropriate workflow will depend on the structure, history, documentation, and intended destination of each dataset.

## Repository structure

Key files and directories include:

```text
.
├── chapters/          # Quarto source files for guidebook chapters
├── images/            # Figures, diagrams, and screenshots
├── templates/         # Templates and other downloadable materials
├── _quarto.yml        # Quarto book configuration
├── index.qmd          # Guidebook landing page
└── README.md          # Repository overview
```

Additional project files support rendering and maintenance of the guidebook.

## Running the guidebook locally

You do **not** need to clone this repository or install R to use the guidebook. Most readers should use the rendered online version linked above.

If you want to edit the source files, run the R examples, or render the guidebook locally, you will need:

- [Quarto](https://quarto.org/)
- [R](https://www.r-project.org/) and preferably [RStudio](https://posit.co/download/rstudio-desktop/)
- The R packages used by the chapters you want to run

After cloning or downloading the repository, open the project in RStudio or a terminal and render the book with:

```bash
quarto render
```

You can preview the guidebook locally while editing with:

```bash
quarto preview
```

R packages are introduced where they are used in the guidebook. If a package required by a code example is not installed on your computer, install it using the standard R package installation process.

## Reproducibility

Code examples are written so that readers can adapt them to their own data rescue projects rather than reproduce a single fixed analysis.

Where possible, the guidebook emphasizes:

- Preserving original source data
- Using scripts rather than manual edits for data transformations
- Using relative rather than absolute file paths
- Keeping data cleaning and validation steps reproducible
- Recording assumptions and decisions in project documentation
- Separating source data, working files, and final outputs
- Checking important assumptions programmatically
- Rerunning workflows from a clean session before treating outputs as final

Package versions used to develop and render the guidebook may differ from those installed by individual readers.

## DataStream workflows

Several chapters provide workflows specifically for preparing freshwater monitoring data for publication on [DataStream](https://datastream.org/).

These chapters use fictional and simplified example datasets to demonstrate common tasks such as:

- Reviewing dataset-level and observation-level metadata
- Mapping source characteristics, units, methods, and monitoring locations to DataStream fields
- Preparing data that follow the DataStream data schema
- Reviewing detection-limit information
- Performing basic QA/QC and pre-upload checks
- Preparing files for review by data owners and data stewards

These examples are intended as reference workflows rather than universal instructions. DataStream requirements and guidance may change over time, so users should also consult DataStream's current documentation when preparing datasets for publication.

## Feedback and contributions

This guidebook is an evolving resource.

If you identify an error, unclear explanation, broken link, or other opportunity to improve the guidebook, feedback is welcome through the GitHub repository [report an issue feature](https://github.com/brcurrinder/ldp-data-rescue-guide/issues/new), or through the Living Data Project team.

## About the Living Data Project

The [Living Data Project](https://livingdata.ca/) is a Canadian Institute of Ecology and Evolution initiative that provides training in data rescue, data management, reproducible research, synthesis, and collaboration while increasing the accessibility and reuse of ecological data.