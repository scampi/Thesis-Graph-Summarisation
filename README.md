# Thesis of Stéphane Campinas

Submitted on August 2016 and accepted on June 2017, at the National University of Ireland, Galway.

## Title

Graph Summarisation of Web Data: Data-driven Generation of Structured Representations

## Abstract

The advent of the Internet enabled the sharing of information between people all around the world. Projects like _Wikipedia_ have made human knowledge accessible to anybody with a simple mouse click. The Linked Data movement has made a considerable leap in the amount of data now available on the Web. Data about science, social interactions, governments, entertainment and more is now available to anybody.

That data is described at a very fine granularity, allowing to describe precisely entities (people, films, monuments, ...) and their relationships. This marks a shift in data management on the Web: instead of a graph of web documents, we witness now a graph of entities with links carrying semantic; we call this _Web Data_.

Web Data is characterized by the use of the Resource Description Framework data model, which enables a dynamic management of information, allowing anyone to easily create and modify data.
That flexible model facilitated the creation of data that grew organically: the structure of the data is not necessarily maintained over time, and some data may be created by integrating several existing datasources, impacting on the structure consistency of the resulting integration. This data is referred to as _semi-structured_.

Web Data is therefore a large collection of semi-structured and heterogeneous data. It is then difficult for a user to understand what information is contained in a particular dataset within that collection or how to access it. In relational database systems, the schema answers to that need; which, in the context of Web Data, is generally missing.

In this thesis, we propose the use of _graph summarisation_ for highlighting the structure of a dataset, which output is referred to as the _graph summary_. The graph summary is a graph, generated from the data itself, which shares the same structure as the original dataset. Unlike the original graph, the summary abstracts itself from details about entities and is focused on the structure of the graph. Therefore, the graph summary is akin to a schema, which we assume is at the core of many applications such as query optimisation, data exploration, data integration, ... . The generation of a graph summary is then intended to be at the core of such applications within the context of Web Data.

We present a formal model for graph summarisation and how to generate a summary.
We use that model to compute _precise_ summaries using the bisimulation equivalence relation; and we argue for the case of _approximate_ graph summaries as the most viable option for many applications.
Because graph summarisation is a technique applied directly on the data, approximate graph summaries are susceptible to the quality of the data.
Hence, we introduce a model for assessing the precision of a summary with regards to the data.
Finally, we develop applications that leverage summaries to demonstrate their usefulness.
