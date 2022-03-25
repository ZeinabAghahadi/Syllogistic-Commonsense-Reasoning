# Avicenna: Syllogistic Commonsense Reasoning
Syllogism is a common form of deductive reasoning that requires precisely two premises and one conclusion. It is considered as a logical method to arrive at new information. For instance, given that "Avicenna wrote the famous book the Canon of Medicine " and " The Canon of Medicine has influenced modern medicine," it can be concluded that "Avicenna has influenced modern medicine."


The Avicenna corpus is a benchmark for syllogistic NLI and syllogistic NLG: 


- syllogistic NLI: Identifying the possibility of inferring between pairs of inputted sentences. 
- syllogistic NLG: Generating a conclusion sentence for two sentences with a syllogistic relation.







# Tasks and Results





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
```
@article{aghahadi2022avicenna,
  title={Avicenna: a challenge dataset for natural language generation toward commonsense syllogistic reasoning},
  author={Aghahadi, Zeinab and Talebpour, Alireza},
  journal={Journal of Applied Non-Classical Logics},
  pages={1--17},
  year={2022},
  publisher={Taylor \& Francis}
}
```






