# Algorithmic Data Science Report

This repository contains my notebook implementation of the questions asked below.

Scenario
Imagine, you have a collection of d (d > 10) documents each containing at least w (w > 50) English words. For testing purposes, you may wish to construct or collect such a collection. A document can be represented as a bag-of-words, i.e., as the set of the words it contains together with associated frequencies. This is most naturally stored using a Python dictionary - and this is called a sparse representation of the data. Alternatively, the dictionary can be converted to a  vector (e.g., a numpy array) where there is a dimension for each of the V words in the English vocabulary. This is called a dense representation.

During lab sessions you will have been expected to have implemented various algorithms that will enable you to address each of the following five questions:

Present an analysis of the theoretical running time of Jaccard’s similarity measure applied to large documents represented as bags of words (in a Python dictionary). Test your analysis empirically by timing and plotting various calculations of Jaccard similarity on your computer. Estimate relevant constants for your implementation and computer.

What is the theoretical worst case running time of the cosine similarity measure applied to documents represented as (dense representation) vectors? Show that this is the case empirically. Estimate the constant for your implementation and computer. Compare using the implementation of the dot product in numpy with your own implementation.

Write a function which computes cosine similarity directly from sparse (dictionary) representations without converting them into dense (vector) representations. Test your function for correctness and compare its efficiency theoretically and empirically to (i) your previous implementation of the cosine similarity, and (ii) your implementation of Jaccard’s measure.

Write a function which computes all-pairs similarities for a collection of documents. The function should take a list of dictionaries (the document collection) and a parameter specifying the similarity measure to be used. What is the theoretical worst-case running time for computing all-pairs similarities? Does it matter what the similarity measure is? Can you give an estimate of how long it would take to compute all-pairs similarities for 200K documents for both measures? (Note: that whilst you should test your function for all-pairs similarities (with d > 10), you do not need to prove the theoretical worst case empirically or test with 200K documents!)

Write a function that implements all-pairs similarities for documents and uses some form of parallel computing, e.g. MapReduce. Make sure you test your function empirically for correctness and for efficiency. Investigate the number of parallel processes that gives optimal results for your implementation and computer.
