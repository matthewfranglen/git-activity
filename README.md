Git Activity
============

git-activity [OPTIONS] URL

This gets the commit activity for the github page provided.

OPTIONS:
  -l COUNT
  --limit COUNT
    Limit commits to the last COUNT days.

Examples
--------

Just getting the data:

    git-activity matthewfranglen
    git-activity https://github.com/matthewfranglen

Limiting the days:

    git-activity -l 7 matthewfranglen
    git-activity --limit 7 matthewfranglen

Graphing the data with [spark](https://github.com/holman/spark):

    git-activity --limit 7 matthewfranglen | spark
