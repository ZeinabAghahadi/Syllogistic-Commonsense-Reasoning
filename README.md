# Avicenna: Syllogistic Commonsense Reasoning
Syllogism is a common form of deductive reasoning that requires precisely two premises and one conclusion. It is considered as a logical method to arrive at new information. For instance, given that "Avicenna wrote the famous book the Canon of Medicine " and " The Canon of Medicine has influenced modern medicine," it can be concluded that "Avicenna has influenced modern medicine."


The Avicenna corpus was developed as a benchmark for syllogistic NLI and syllogistic NLG.


Avicenna contains 6,000 records for binary classification, 3000 of them with a syllogistic relation, and the other 3000 with no syllogistic relation.


- syllogistic NLI: Identifying the possibility of inferring between pairs of inputted sentences. 
- syllogistic NLG: Generating a conclusion sentence for two sentences with a syllogistic relation.


3,000 of sentence pairs have a syllogistic relation present and in the remaining 3000 records a syllogistic relation is absent. 





# Results
Please refer to the manuscript for more results.





## 1. Syllogistic NLI 

Model| Test Acc. (%) 
 -----|------
 Baselines:| 
 Random label | 50.16   
 Manhattan LSTM | 51.50
 ESIM + ELMO |66.90
 Partial input:| 
 Fine-tuned BERT with Avicenna [minor premise Only] | 59.33
 Fine-tuned BERT with Avicenna [major premise Only] |59.83
 Pre-trained LMs:|
 Base BERT (BERT pre-trained model classification)| 56.75
 BERT Based Avicenna-trained model|87.69
 XLNet Based Avicenna-trained model |89.19
 Adversarial BERT Based Avicenna-trained model|89.68
 Adversarial XLNet Based Avicenna-trained model |92.19
 Human Performance:|98.16
 
 
 ## 2. Syllogistic NLG
 
 
 Model| BLEU | ROUGE | BERT-Score | Human Acc. (%) 
 -----|------| ------| ---------  |--------------  
 RNN LSTM| 0.60| 3.80 | 76.5  |-  
 Fine-tuned Gpt-2 with Avicenna_Direct | -      |  - |   -|11   
 Fine-tuned Gpt-2 with Avicenna_with classification | 53.3      |  50.1 |   92.4|31.2  
 Fine-tuned Gpt-2 with middle-term dataset (Transfer learning) | 54.3      |  54.2 |   92.5|32.0   
 



# Bibtex

@article{aghahadi2022,
  title={Avicenna: A Challenge Dataset for Natural Language Generation toward Commonsense Syllogistic Reasoning},
  author={Zeinab Aghahadi, Alireza talebpour},
  journal={Journal of Applied Non-Classical Logics},
  year={2022},
  publisher = {Taylor and Francis}
} 


