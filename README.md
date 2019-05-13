# Learned Sectors

Final project report for FE 800 (Special Research Problems) to fulfill graduation requirements for the Master of Science in Financial Engineering at the Stevens Institute of Technology.

Completed in May 2019.


## Style Guide

### Package Imports

Put all LaTeX package imports in the [resources/header.tex](resources/header.tex) file, with a comment explaining what it is for. All current imports are in alphabetical order.

### Citations

Always wrap citations in the `\citeFormat{}` LaTeX command.

Example: **\citeFormat{\cite{Weerawarana2016}}**



## Contribution Guidelines

**General Note:** Sensibly name files.

### Creating new Sections

Always create new sections in the `sections/` folder; see [sections/sample_section.tex](sections/sample_section.tex).

### Naming Conventions

Naming conventions for figure, table, appendix, and cross-references:

*Note*: Replace spaces in chapter names with underscores (_).

|Type|Structure|Example|
|:--:|:-------:|:-----:|
|Figure|`fig:chapter_name:fig_name`|`fig:literature_review:article_architecture_diagram`|
|Table|`tab:chapter_name:table_name`|`tab:literature_review:table_name`|
|Appendix|`appendix:appendix_name:item_name`|`appendix:backtest_data:portfolio_value`|
|Cross-References (Titles/Important Things)|`chapter_name:item_name`|`research_goals:clustering`|

### GitHub Commits

Because this is connected to my (Rukmal's) GitHub account on overleaf, *always* preface all commit messages from Overleaf to GitHub with your name in square brackets.

Example: **[rukmal] updated README**

## Viewing the Project

This report was developed on Overleaf. A read-only view is available at the following URL:

https://www.overleaf.com/read/dtwmbwfgxtcq

## Contact

[Rukmal Weerawarana](http://rukmal.me)