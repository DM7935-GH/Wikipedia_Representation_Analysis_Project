# Wikipedia Representation Analysis Project
This repository contains the code for my dissertation project, titled "Analysing the Representation of Historical Figures
on Wikipedia Using Computational Methods". It also includes examples of input data (for the analysis programs), and a sample of the results files and visualisations produced by the code.


## Project Description
### Background
Wikipedia is one of the most popular digital sources of information, which gives it a significant amount of influence over how topics are represented online. The articles in Wikipedia's 340+ language editions are created and edited by volunteers from across the world.  

However, overall contribution to the website is dominated by people from more developed countries. Representations of the same topic (in terms of the information included, opinions expressed, and tone) often differ across language editions, raising the question of whether some perspectives are more influential than others.

### Objectives
The project aims to investigate:  
- Whether the representation of important historical figures (specifically, from the Cold War era) varies between different editions of Wikipedia.  
- Which countries' Wikipedia editors contribute the most to these articles.  

### Data Collection
12 prominent Cold War figures were chosen for this project, with 3-5 article editions (the version of an article in a given language edition) being selected for each figure.  

For each article edition, the dataset included:  
- The plaintext content of the article.  
- Specific data on every edit made to the article, including the edit timestamp and IP address of the editor.  

<img width="500" height="170" alt="Image" src="https://github.com/user-attachments/assets/2390d8e9-77a9-491f-b7ec-fcf532225270" />  

### Analysis Methodology
The content of each article edition was analysed using Natural Language Processing (NLP) methods:  
- Paragraph-level sentiment analysis (to measure the overall tone/sentiment).  
- Aspect-based sentiment analysis (to measure sentiment towards certain aspects).  
- LDA topic modelling (to identify the most prominent topics).

The edit data for each article edition was analysed based on frequency:  
- IP addresses were geolocated to assess the global distribution of editors.
- Timestamps were used to assess the temporal distribution of edits.

<img width="800" height="400" alt="Image" src="https://github.com/user-attachments/assets/536907d5-4491-41bc-80cb-4631006280ae" />  

The analysis results for each Cold War figure were compiled and visualised, in order to interpret and compare them more easily. Two examples are given below:  

<img width="800" height="430" alt="Image" src="https://github.com/user-attachments/assets/2233023a-6155-4f85-9800-001bebdbe505" />  
<img width="800" height="400" alt="Image" src="https://github.com/user-attachments/assets/135f69f3-49fc-4e90-82a4-9b8f27484df6" />  


## Repository Contents
- `Project_Code` - Contains the project code files.
- `Example_Input_Data` - Contains a sample of the article content and edit data files produced by the data collection programs (for John F. Kennedy's Wikipedia article).
- `Sample_Results` - Contains a sample of the project results files produced by the analysis programs (for John F. Kennedy's article).


## Attribution
Sources of data:  
- Wikipedia articles (plaintext only)  
- Wiki Replicas databases (data extracted via Wikimedia's (Quarry)[https://meta.wikimedia.org/wiki/Research:Quarry] and (PAWS)[https://wikitech.wikimedia.org/wiki/PAWS] services)  

NLP models used:
- (cardiffnlp/twitter-xlm-roberta-base-sentiment)[https://huggingface.co/cardiffnlp/twitter-xlm-roberta-base-sentiment] (Hugging Face)  
- (pilardi/sentiment-analysis:llama3 )[https://ollama.com/pilardi/sentiment-analysis:llama3] (Ollama)  


## License
The contents of the `Article_Text` files within the `Example_Input_Data` folder were sourced from Wikipedia, and are thus licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).  

All other materials within this repository are licensed under the MIT License.  

See the `LICENSE` and `LICENSE-CC-BY-SA` files for the full license texts.  
