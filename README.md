# Seminar4012
# Transfer Learning for Text Classification with Tensorflow
Tensorflow implementation of Semi-supervised Sequence Learning(https://arxiv.org/abs/1511.01432).

   1) SA-LSTM: Use auto-encoder as a pre-trained model.
   
   2) LM-LSTM: Use language model as a pre-trained model.
# Requirements

  Python 
  Tensorflow
  pip install -r requirements.txt
# Usage

DBpedia dataset is used for pre-training and training.
# Pre-train auto encoder or language model

`python pre_train.py --model="<MODEL>"`

(\<Model>: auto_encoder | language_model)
# Train LSTM text classification model

`python train.py --pre_trained="<MODEL>"`

(\<Model>: none | auto_encoder | language_model)
# Experimental Results

  Orange lines: LSTM
  
  Blue lines: SA-LSTM
  
  Red lines: LM-LSTM

# Loss
![42726945-089634b0-87d8-11e8-8f3e-0e986f1d4b51](https://user-images.githubusercontent.com/102894040/217367388-47d9dcea-8279-4b9d-b58f-5460509fb3a4.PNG)
# Accuracy
![42726944-073e19e8-87d8-11e8-8a60-788fb109ea11](https://user-images.githubusercontent.com/102894040/217367553-93381cb7-90c8-428c-b2fe-615b61845a6a.PNG)
