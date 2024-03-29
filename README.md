# Sars-Covid-19--knowledge-graph-LLMs
AI Prompt Engineer Internship  [ Docu3c ]

Problem Statment :
Decoding Covid-19 with Genome Analysis using knowledge graph

Overview Given problem statement 
You are one of the researchers responding to the White House Office of Science and Technology Policy center’s call to conduct advanced research on Covid-19. You are working with CDC, which has led a coordinated effort to set up a machine readable dataset. A dataset that represents the most extensive machine-readable coronavirus literature collection available for data and text mining to date, with over 29,000 articles, more than 13,000 of which have full text. Using the CORD-NER dataset and Knowledge Graph, determine and map out the details of the SARS-CoV-2 genome to assist understanding of the emergence, evolution and diagnosis of this deadly virus.


knowledge graphs in machine learning :
A knowledge graph, also known as a semantic network, represents a network of real-world entities—i.e. objects, events, situations, or concepts—and illustrates the relationship between them. This information is usually stored in a graph database and visualized as a graph structure, prompting the term knowledge “graph.”


Dataset Link :
https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge


Simple procedure :

I have created the solution for above mentioned problem using LLMs (Langchain from Huggingface) for NER Model and developed a knowledge graph using the Entities, Relations and Edges.

1. Import the necessary libraries such as (Example: transformers, sentencepiece, langchain, HuggingFacePipeline, AutoTokenizer, networkx, matplotlib, etc)
2. Import the Dataset specific file named Metadata.csv (1.65 GB) , The whole Dataset contains 87 GB of Data which makes the model hard to execute. So filter the neccessary data and import it.
3. Then using the imported libraries , Prompt & Pre-trained model such as transformers,Universal-NER/UniNER-7B-all. we need to extract the Entities & Relationships.
4. By changing the parameters of Pre-trained Model & Prompt value we can collect the Entities & Labels.
5. By using matplotlib, networkx libraries draw the knowledge graphs for the Entities with Relationships & edges.
6. plot the output of Knowledge Graph.


Article refered regarding genetic structure of SARS-CoV-2 :
https://onlinelibrary.wiley.com/doi/full/10.1002/bies.202000240


Sample Output :
![s1](https://github.com/PraveenSP12/Sars-Covid-19---knowledge-graph-LLMs-/assets/95535247/71afd054-312d-481b-bb3b-c4e5da46eabb)
![s2](https://github.com/PraveenSP12/Sars-Covid-19---knowledge-graph-LLMs-/assets/95535247/a0202ad4-f156-4385-a9c3-934ef4dd81b3)
![s3](https://github.com/PraveenSP12/Sars-Covid-19---knowledge-graph-LLMs-/assets/95535247/8ca71990-d292-4b11-b56c-c7c634efcde3)
![s4](https://github.com/PraveenSP12/Sars-Covid-19---knowledge-graph-LLMs-/assets/95535247/ecb5774b-caf2-4255-8048-134b71406d61)
