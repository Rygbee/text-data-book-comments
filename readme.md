# Text Data Analysis and Management: A Practical Introduction to Text Mining and Information Retrieval

by [ChengXiang Zhai](http://web.engr.illinois.edu/~czhai/) and [Sean
Massung](http://web.engr.illinois.edu/~massung1/), [University of Illinois Computer Science Department](http://cs.illinois.edu/)

## Introduction

Recent years have seen a dramatic growth of natural language text data,
including web pages, news articles, scientific literature, emails, enterprise
documents, and social media such as blog articles, forum posts, product reviews,
and tweets. This has led to an increasing demand for powerful software tools to
help people analyze and manage vast amounts of text data effectively and
efficiently. Unlike data generated by a computer system or sensors, text data
are usually generated directly by humans, and are accompanied by semantically
rich content. As such, text data are especially valuable for discovering
knowledge about human opinions and preferences, in addition to many other kinds
of knowledge that we encode in text. In contrast to structured data, which
conform to well-defined schemas (thus are relatively easy for computers to
handle), text has less explicit structure, requiring computer processing toward
understanding of the content encoded in text. The current technology of natural
language processing has not yet reached a point to enable a computer to
precisely understand natural language text, but a wide range of statistical and
heuristic approaches to analysis and management of text data have been developed
over the past few decades. They are usually very robust and can be applied to
analyze and manage text data in any natural language, and about any topic.

This book provides a systematic introduction to all these approaches, with an
emphasis on covering the most useful knowledge and skills required to build a
variety of practically useful text information systems. The focus is on text
mining applications that can help users analyze patterns in text data to extract
and reveal useful knowledge. Information retrieval systems, including search
engines and recommender systems, are also covered as supporting technology for
text mining applications. The book covers the major concepts, techniques, and
ideas in text data mining and information retrieval from a practical viewpoint,
and includes many hands-on exercises designed with a companion software toolkit
(i.e., [MeTA](http://meta-toolkit.github.io/meta/)) to help readers learn how to
apply techniques of text mining and information retrieval to real-world text
data and how to experiment with and improve some of the algorithms for
interesting application tasks. The book can be used as a textbook for a computer
science undergraduate course or a reference book for practitioners working on
relevant problems in analyzing and managing text data.

## Part I: Overview and Background

This part provides an overview of the motivation and high-level concepts of the
book, and gives readers a roadmap for navigating through the chapters in the
later parts. It also includes a background chapter where basic concepts in
probability and statistics, machine learning, and natural language processing
are introduced so that readers without any knowledge in these areas will have
the necessary background to understand the materials later. This part further
includes one chapter on the [MeTA](http://meta-toolkit.github.io/meta/) toolkit,
which will be the basis for many exercises later. We use this chapter to
introduce the typical architecture of a text mining system, where the search
engines will be shown as a basis for supporting text analysis. Readers with
sufficient background knowledge about these topics can skip part or all of this
section.

1. Introduction
  1.1 Text data vs. structured data
  1.2 Text data analysis and management
  1.3 How to use this book

2. Background
  2.1 Basics of probability and statistics
  2.2 Basics of machine learning
  2.3 Natural language processing and text representation

3. MeTA: A Modern Data Sciences Toolkit
  3.1 Design philosophy
  3.2 Architecture
  3.3 Uses of MeTA
  3.4 Exercises

## Part II: Text Data Access

Text data access is the foundation for text analysis. Text access technology
plays two important roles in text analysis and management applications. First,
it enables retrieval of the most relevant text data to a particular analysis
problem, thus avoiding unnecessary overhead from processing a large amount of
non-relevant data. Second, it enables interpretation of any analysis results or
discovered knowledge in appropriate context and provides data provenance. The
general goal of text data access is to connect users with the right information
at the right time. This connection can be done in two ways: *pull*, where the
users take the initiative to fetch relevant information out from the system, and
*push*, where the system takes the initiative to offer relevant information to
users. The main technology supporting *pull* is search engines which are covered
in detail in one long chapter. The main technology supporting *push* is
recommender systems, covered in a later chapter. The chapter Interactive
Information Access* will cover how the pull and push modes can be integrated in
an interactive hybrid system, providing a unified view of text data access.

4. Overview of text data access
  4.1 Access mode: pull vs. push
  4.2 Querying vs. browsing
  4.3 Multimode interactive access

5. Search engines
  5.1 Basic concepts of search engines
  5.2 Information retrieval models
  5.3 Implementation of search engines
  5.4 Evaluation
  5.5 Advanced techniques for improving search engines
  5.6 Web search engines
  5.7 Exercises

6. Recommender systems
  6.1 Content-based recommendation
  6.2 Collaborative filtering
  6.3 Hybrid recommender systems
  6.4 Evaluation
  6.5 Applications
  6.6 Exercises

## Part III: Text Data Analysis

This part covers a variety of techniques for text data analysis, where the goal
is to analyze text data to find interesting semantic patterns and extract
useful knowledge. We cover algorithms for four basic text analysis tasks,
including text clustering, text categorization, text summarization, and topic
analysis, each covered in one chapter. The last chapter of this part takes a
broader view of the problem of text analysis by placing it in the context of
joint analysis of text and structured data, which is generally needed in an
application scenario where we have available both unstructured text data and
companion structured data, and would prefer analyzing all the data for solving
a particular application problem.

7. Overview of text data analysis
  7.1 Text analysis vs. text management
  7.2 Deep analysis vs. shallow analysis
  7.3 A conceptual framework for text analytics

8. Text clustering
  8.1 Overview of clustering techniques
  8.2 Document clustering
  8.3 Term clustering
  8.4 Evaluation
  8.5 Applications
  8.6 Exercises

9. Text categorization
  9.1 Overview of text categorization techniques
  9.2 Features for text categorization
  9.3 Evaluation
  9.4 Applications
  9.5 Exercises

10. Topic analysis
  10.1 Overview of topic analysis techniques
  10.2 Basic topic models
  10.3 Advanced topic models
  10.4 Evaluation
  10.5 Applications
  10.6 Exercises

11. Text summarization
  11.1 Overview of text summarization techniques
  11.2 Extractive text summarization
  11.3 Abstractive text summarization
  11.4 Query-specific text summarization
  11.5 Evaluation
  11.6 Applications
  11.7 Exercises

12. Joint analysis of text and structured data
  12.1 Context and companion structured data of text
  12.2 Contextualized text analysis
  12.3 Integrated analysis of text and structured data
  12.4 Evaluation
  12.5 Applications
  12.6 Exercises

## Part IV: Application System Development with MeTA

This last part of the book discusses how to use MeTA to develop an application
system for text analysis and management. It has two chapters. The first is
about a unified conceptual framework for integrating text data access and text
data analysis and preliminary ideas about how to design an algebra for text
analysis with multiple analysis operators that can be combined in a flexible
way to support different analysis workflows. The second is a detailed
discussion of how different components in MeTA can be combined in interesting
ways to support complex analysis workflows; it helps readers learn how to use
or adapt MeTA to develop useful text information systems to solve their
specific application problems. The last chapter provides information about how
people can contribute to the development of MeTA, which we expect to be an
ongoing effort with a dedicated website and regular open source releases.

13. A unified conceptual framework for text analysis
  13.1 An algebra for text analytics
  13.2 Implementation of analysis operators
  13.3 Workspace management
  13.4 Workflow support and optimization

14. MeTA for text analysis and management
  14.1 Overview of MeTA modules
  14.2 MeTA API
  14.3 Other text analysis and management toolkits
  14.4 Sample applications

15. Contributing to MeTA
