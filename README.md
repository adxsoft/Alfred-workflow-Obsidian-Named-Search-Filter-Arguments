# Alfred-workflow-Obsidian-Named-Search-Filter-Arguments

Obsidian Graph or Filter Alfred Workflow

# 1. Why have I created this workflow?

In Obsidian 12.11 search arguments and graph filters are not easily able to be recalled by name. 
This alfred workflow allows you to define your default search/filter arguments and insert them wherever you need in the search and filter input fields.

My default search arguments are

xxx -path:"Daily Notes" -path:"Templates" -path:"Templater" -file:"01 - My Schedule.md" -file:"04 - Project Review.md" -file:"05 - Someday.md" -Assets -Zettelkasten

where xxx is my simple search of graph filter argument so I often need to enter a search like

golf pitching -path:"Daily Notes" -path:"Templates" -path:"Templater" -file:"01 - My Schedule.md" -file:"04 - Project Review.md" -file:"05 - Someday.md" -Assets -Zettelkasten

to be able to have a nicely filtered graph for golf and pitching notes

# 2. This Workflow has two snippet triggers ::sarg and ::slist

::sarg alfred command will
- paste in the standard search path defined in the args and vars block variable 'standardgraphfilter'


::slist alfred command will
- display a list of choices of named search argument
- the choices are defined in the Graph Filter Component of the workflow
    - each item in the Graph Filter has a search/filter argument eg 'Golf Pitching {var:dailynotesonly}'
- any number of choices can be set up
