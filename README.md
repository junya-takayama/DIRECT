# DIRECT: Direct and Indirect REsponses in Conversational Text Corpus

We create a large-scale dialogue corpus that provides pragmatic paraphrases to advance technology for understanding users' nonverbal intentions.  
Our corpus provides a total of 71,498 indirect-direct utterance pairs accompanied by a multi-turn dialogue history extracted from the MultiWoZ dataset. 

train.csv consists of five columns except for the index column.

| column name        | description                                                   | 
| ------------------ | ------------------------------------------------------------- | 
| dialogue_id        | The corresponding dialogue ID in the MultiWoZ data            |
| turn_index         | The position of the utterance in the dialogue (0-based index) | 
| target_utterance   | The original utterance extracted from the MultiWoZ data      | 
| direct_utterance   | Collected direct response                                     | 
| indirect_utterance | Collected indirect responses                                  | 

In addition to the above columns, test.csv contains the quality evaluation results.

| column name           | description                                                                                           | 
| --------------------- | ----------------------------------------------------------------------------------------------------- | 
| isacceptable_direct   | Whether direct_utterance is considered to be the same intention as target_utterance (TRUE / FALSE)   | 
| isacceptable_indirect | Whether indirect_utterance is considered to be the same intention as target_utterance (TRUE / FALSE) | 
| quality               | Whether direct_utterance is more direct than indirect_utterance (Good / Neutral / Bad)                | 

