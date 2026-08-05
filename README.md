# Wikipedia Representation Analysis Project
This repository contains the code for my dissertation project, titled "Analysing the Representation of Historical Figures
on Wikipedia Using Computational Methods". It also includes examples of input data (for the analysis programs), and a sample of the results files and visualisations produced by the code.


## Project Description
#### Background
Wikipedia is one of the most popular digital sources of information, which gives it a significant amount of influence over how topics are represented online. The articles in Wikipedia's 340+ language editions are created and edited by volunteers from across the world.  
However, overall contribution to the website is ![alt text](image.png)dominated by people from more developed countries. Representations of the same topic (in terms of the information included, opinions expressed, and tone) often differ across language editions, raising the question of whether some perspectives are more influential than others.

#### Objectives
The project aims to investigate:  
- Whether the representation of important historical figures (specifically, from the Cold War era) varies between different editions of Wikipedia.  
- Which countries' Wikipedia editors contribute the most to these articles.  

#### Data Collection
12 prominent Cold War figures were chosen for this project, with 3-5 article editions (the version of an article in a given language edition) being selected for each figure.  

For each article edition, the dataset included:  
- The plaintext content of the article.  
- Specific data on every edit made to the article, including the edit timestamp and IP address of the editor.  

#### Analysis Methodology
The content of each article edition was analysed using Natural Language Processing (NLP) methods:  
- Paragraph-level sentiment analysis (to measure the overall tone/sentiment).  
- Aspect-based sentiment analysis (to measure sentiment towards certain aspects).  
- LDA topic modelling (to identify the most prominent topics).

The edit data for each article edition was analysed based on frequency:  
- IP addresses were geolocated to assess the global distribution of editors.
- Timestamps were used to assess the temporal distribution of edits.

The analysis results for each Cold War figure were compiled and visualised, in order to interpret and compare them more easily.  


## Contents
WIP.  


## License
WIP.  


## Attribution
WIP.  
