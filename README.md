# Ad hoc checklist of alien species in Belgium

## Rationale

This repository contains the functionality to standardize the _Ad hoc checklist of alien species in Belgium_ (a list of alien species that are not yet included in authorative checklists) to a [Darwin Core checklist](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org).

## Workflow

[source data](https://github.com/trias-project/ad-hoc-checklist/blob/master/data/raw) (maintained as a [Google Spreadsheet](https://docs.google.com/spreadsheets/d/1LeXXbry2ArK2rngsmFjz_xErwE1KwQ8ujtvHNmTVA6E/edit#gid=0)) → Darwin Core [mapping script](https://trias-project.github.io/ad-hoc-checklist/dwc_mapping.html) → generated [Darwin Core files](https://github.com/trias-project/ad-hoc-checklist/blob/master/data/processed)

## Published dataset

* [Dataset on the IPT](https://ipt.inbo.be/resource?r=ad-hoc-checklist)
* [Dataset on GBIF](https://doi.org/10.15468/3pmlxs)

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) and the [Checklist recipe](https://github.com/trias-project/checklist-recipe). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md              : Description of this repository
├── LICENSE                : Repository license
├── ad-hoc-checklist.Rproj : RStudio project file
├── .gitignore             : Files and directories to be ignored by git
│
├── data
│   ├── raw                : Source data (from Google Spreadsheet), input for mapping script GENERATED
│   └── processed          : Darwin Core output of mapping script GENERATED
│
├── docs                   : Repository website GENERATED
│
└── src
    ├── dwc_mapping.Rmd    : Darwin Core mapping script, core functionality of this repository
    ├── _site.yml          : Settings to build website in docs/
    └── index.Rmd          : Template for website homepage
```

## Installation

1. Clone this repository to your computer
2. Open the RStudio project file
3. Open the `dwc_mapping.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio
4. Install any required packages
5. Click `Run > Run All` to generate the processed data
6. Alternatively, click `Build > Build website` to generate the processed data and build the website in `docs/`

## Contributors

[List of contributors](https://github.com/trias-project/ad-hoc-checklist/contributors)

## License

[MIT License](https://github.com/trias-project/ad-hoc-checklist/blob/master/LICENSE)
