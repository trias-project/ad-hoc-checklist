# Ad hoc checklist of alien species in Belgium

## Rationale

<!-- This section gives a quick description of what this repository is for. At least update the "... the data of (blank) ..." or edit as you see fit. -->

This repository contains the functionality to standardize the _Ad hoc checklist of alien species in Belgium_ (a list of alien species that are not yet included in authorative checklists) to a [Darwin Core checklist](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org).

## Workflow

[source data](data/raw) (maintained as a [Google Spreadsheet](https://docs.google.com/spreadsheets/d/1LeXXbry2ArK2rngsmFjz_xErwE1KwQ8ujtvHNmTVA6E/edit#gid=0)) → Darwin Core [mapping script](src/dwc_mapping.Rmd) → generated [Darwin Core files](data/processed)

## Published dataset

* [Dataset on the IPT]()
* [Dataset on GBIF]()

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) and the [Checklist recipe](https://github.com/trias-project/checklist-recipe). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md              : Description of this repository
├── LICENSE                : Repository license
├── ad-hoc-checklist.Rproj : RStudio project file
├── .gitignore             : Files and directories to be ignored by git
│
├── data
│   ├── raw                : Source data, input for mapping script
│   └── processed          : Darwin Core output of mapping script GENERATED
│
├── docs                   : Repository website GENERATED
│
└── src
    ├── dwc_mapping.Rmd    : Darwin Core mapping script, core functionality of this repository
    ├── _site.yml          : Settings to build website in /docs
    └── index.Rmd          : Template for website homepage
```

## Installation

1. Clone this repository to your computer
2. Open the RStudio project file
3. Open the `dwc_mapping.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio
4. Install any required packages
5. Click `Run > Run All` to generate the processed data
6. Alternatively, click `Build > Build website` to generate the processed data and build the website in `/docs` (advanced)

## Contributors

[List of contributors](https://github.com/trias-project/ad-hoc-checklist/contributors)

## License

[MIT License](LICENSE)
