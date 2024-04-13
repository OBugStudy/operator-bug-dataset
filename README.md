# Operator Bug Dataset

This is the dataset for the ISSTA`24 submission "An Empirical Study on
Kubernetes Operator Bugs". It contains 208 operator bugs collected
from popular Kubernetes operators. 

## Getting started 
You can directly use the dataset for further analysis, including bug
detection, bug fix, etc. All details are included in the file
`dataset.xlsx`.

## Detailed description
In `dataset.xlsx`, there are four sheets: one main sheet which
contains detailed information for operator bugs and three statistics
sheets for summary.

We explain the meaning of information row in the main sheet `Bug
Details` as follows:
- Bug ID: we name each bug according to the criteria:
  - If the issue has given the bug a name, we apply it.
  - Else we put together the project's name and issue's id to generate
    the ID.
- Issue link: the original link for the bug issue.
- Title: issue title for the bug.
- PR Link: the link for pull request which fixes the bug.
- Root Cause: there can be up to three levels for bug root causes,
  each of which is connected by right arrow:
  - Main dimension: describe the main bug pattern.
  - Category: we further categorize operator bugs into different
    categories, except for the ACM configuration.
  - Sub category: characterize bugs at a finer level of granularity.
- Manifestation: contains the factors which contribute to the
  triggering of operator bugs.
- Resources: resources involved in the triggering of operator bugs.
- Scenario: we split the reproduction steps for operator bugs into
  several steps to help further researchers to revisit them more
  easily.
- Impacts: operator bugs could have multiple impacts at the same time
  and each of the impact is connected by the forward slash.
- Fix: brief description of the fix strategies used to fix the bug.