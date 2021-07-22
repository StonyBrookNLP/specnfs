**SpecNFS** dataset is a collection of 1198 setences annotated with their **SpecIR** representation. This dataset is part of our paper **SpecNFS: A Challenge Dataset Towards Extracting Formal Models from Natural Language Specifications**, which can be found in **SpecNFS-NLP4prog.pdf**.

The datasets in **SpecNFS** along with their brief description are as follows:

<ol>
 
<li> ./dataset/NER_dataset.csv

This is the dataset containing the information about the spans and type of the entities in a sentence

| **Column**   |  **Description** | 
| --- | ---- |
| Sentence  |  Sentence number | 
| Token     |  Token in the sentence | 
| Token_ID  |  Unique identifier of the span of entity in a sentence | 
| Token_no  |  Sequence number of a token in a sentence. | 
| Partition |  The partition no. of the sentence which was used for the 5-fold cross validation reported in the paper  |

 </li>
 
<li> ./dataset/Link_dataset.csv

This is the dataset containing dependency link information between entities in a sentence

| Column       |  Description |
| --- | ---  |
| Head_id      |  Entity span identifier of the head of the link  |
| Dep_id       |  Entity span identifier of the dependent of the link  |
| Link         |  Type of link between the head and the dependenct entity  |
| Sentence_no  |  Sentence number of the link  |
| Partition    |  The partition no. of the sentence which was used for the 5-fold cross validation reported in the paper   |

</li>

<li> ./dataset/token_type2link_type.csv 

This is the dataset containing the valid link types between different pair of entity types

 | Column       |  Description  | 
 | ---  | ---  | 
 | H_Token_TYPE | Head entity type  | 
 | D_Token_TYPE | Dependenct entity type  | 
 | Link_TYPE    | Valid link types between head and dependenct entity types  | 

 </li>

</ol>
