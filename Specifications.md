# Project Outline

Superlatives are praises usually given to students by their classmates at the end of the school year. A person gets a superlative by being getting the most votes in a category from their peers. An example of a superlative would be "Best dressed".

This application splits the voting into two parts: nomination and the actual voting. The nomination will be done by a few members of the larger group where everyone gets nominated for at least five categories. The actual voting is then done by everyone where every category has five nominees.

This means that it'll need to store two basic data types, which are: Voters and Categories. From these we'll get the nominators and the electorate. This will be handled by a simple database with a simple backend. It'll be accessed through an api with the following endpoints:
    - /api/contestants/add
    - /api/contestants/remove
    - /api/contestants/all
    - /api/categories/add
    - /api/categories/remove
    - /api/categories/all
    - /api/vote

In terms of presentation, the app will have three stages: welcome page, voting page and the results.
The welcome page will contain a simple introduction to the app, the idea of superlatives, the rules and the process used.
The voting page will be split into nomination and voting. In nomination every user will have their own page with a list of categories from which the nominator can choose to nominate them. In the voting page, each category will have five people with the highest nominations.
The results will be presented accordingly to the categories, this can be output as a document.
    - /welcome
    - /nominate
    - /vote
    - /results

The voting will use a ranked choice system, and will be biased to allow every one be nominated in at least 3 categories. And every candidate gets at most 5 nominations.
