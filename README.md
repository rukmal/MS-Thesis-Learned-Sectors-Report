# Learned Sectors

Final project report for FE 800 (Special Research Problems) to fulfill graduation requirements for the Master of Science in Financial Engineering at the Stevens Institute of Technology.

Completed in May 2019.

## Abstract

> Market sectors play a key role in the efficient flow of capital through the modern Global economy. Their use is widespread across the entire spectrum of market participants and observers, ranging from Governments using them to better regulate industry, to retail investors gaining exposure to particular segments of the economy through exchange traded funds tracking sector indices. We analyze existing sectorization heuristics, and observe that the most popular - the GICS (which informs the S&P 500), and the NAICS (published by the U.S. Government) - are not entirely quantitatively driven, but rather appear to be highly subjective and rooted in dogma.
>
> We examined alternative approaches to market sectorization, and found that returns-based methods were inherently flawed due to the significant bias of existing classifications on the structure of correlation distributions of the returns. Following this, we inspected determinants of firm value that would be intrinsically descriptive of the economic operating domain of a company. Building on inferences from analysis of the capital structure irrelevance principle and the Modigliani-Miller theoretic universe conditions, we postulate that corporation fundamentals - particularly those components specific to the Modigliani-Miller universe conditions - would be optimal descriptors of the true economic domain of operation of a company. Fundamentals data from Form 10-K for 15 features were downloaded for 362 companies in the S&P 500, forming the feature space on which train our classification model.
>
> To this end, we developed a new, objective data-driven sector classification heuristic, based on a HCA algorithm. We utilized this novel heuristic to generate a set of potential candidate learned sector universes, by varying the linkage method of the HCA algorithm (testing SLINK, CLINK, ALC, and WARD linkage methods), and the number of resulting sectors derived from the model (ranging from 5 to 19), resulting in a total of 60 candidate learned sector universes.
>
> We then introduce *reIndexer*, a backtest-driven sector universe evaluation research tool, to rank the candidate sector universes produced by our learned sector classification heuristic. *reIndexer* backtests portfolios of synthetic exchange traded funds, constructed based on the specifications of a candidate sector universe. The backtest period was from January 1st 2012 to December 31st 2017, tracking the evolution of the portfolio daily. The backtest results of each classification universe are then evaluated against each other, to derive a de facto *rank* for the candidate sector universes. This rank was utilized to identify the risk-adjusted return optimal learned sector universe as being the universe generated under CLINK (i.e. complete linkage), with 17 sectors.
>
> Finally, we evaluate our risk-adjusted return optimal learned sector against the benchmark classification heuristic, the GICS S&P 500 Classification. *reIndexer* was used again to backtest the GICS classification universe against the optimal (complete linkage; 17 sectors) learned sector universe. We found that our learned sector universe portfolio outperformed the benchmark with respect to both absolute portfolio value, and the risk-adjusted return of the portfolio over the backtest period.
>
> We conclude that we fully explored the scope of our thesis statement, and addressed our specific research goals through the successful development of a fundamentals-driven Learned Sector classification heuristic with a superior risk-diversification profile than the status quo classification heuristic.


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
