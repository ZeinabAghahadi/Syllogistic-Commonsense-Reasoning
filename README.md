# Avicenna: Syllogistic Commonsense Reasoning
# Result
Please refer to the manuscript for more results.

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
 
 
 
 
 
 
 

 
  
 
 
 Model| BLEU | ROUGE | BERT-Score | Human Acc. (%) 
 -----|------| ------| ---------  |--------------  
 RNN LSTM| 0.60| 3.80 | 76.5  |-  
 Fine-tuned Gpt-2 with Avicenna_Direct | -      |  - |   -|11   
 Fine-tuned Gpt-2 with Avicenna_with classification | 53.3      |  50.1 |   92.4|31.2  
 Fine-tuned Gpt-2 with middle-term dataset (Transfer learning) | 54.3      |  54.2 |   92.5|32.0   
 



# Reference

