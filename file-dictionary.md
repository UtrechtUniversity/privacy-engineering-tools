# File dictionary

This file specifies what information should ideally be in the tables that list available tools. This makes sure, firstly, that users have the necessary information to estimate whether the tool is for them, and secondly, that the files use about the same language to describe the tools. 

## Minimal requirements for the tool list

For each tool, include at minimum:
- Name, linked to the software/tool (`[Name tool](link tool)`)
- Description: a short description of what the tool does
  - Mention if the software is open source and if so, include the link to the code

## Preferable components to include

We prefer that you also include:
- Maintenance: how actively is the software maintained? 
  - Levels: Active (last commit was less than a year ago) / Inactive (last commit was more than a year ago)
  - Only relevant if this information is available
- Number of GitHub stars (this may not always be relevant however)
  - Levels: 0-10, 10-100, 100-500, 500-1000, 1000+
  - Only relevant if the tool is on GitHub
- License + a link to the license if possible
  - We've already come across: MIT / GPL-v2 / GPL-v3 / Apache 2.0 / BSD-3 Clause / BSD-2 Clause / BSD-3 Clause-Clear / EUPL-1.2 / Missing
- More info: where can users find more information? Think of documentation, tutorials, articles, demonstrations, etc.
  - Please make sure you are using persistent identifers where possible, e.g. for a journal article a DOI is preferable.

## More detailed information to include

Dependent on the type of tool, a more structured display of features of the tool may be desired. For example:

- What methods does the tool use (e.g., privacy models, generative models)?
- For what type of data are these tools useful?
- Who are the target audience of the tool?
- What is the result of using the tool? This is especially useful for synthetic data tools.