## A Multilevel Semantic Fusion Relation Detection Model for Knowledge-Based Question Answering

* Introduction
  > The knowledge base question answering (KBQA) is generally decomposed into several subtasks, such as entity recognition, entity linking, relation detection, inference and etc. Relation detection is one of the most critical subtasks in KBQA. To improve the accuracy of relation detection, we propose a multilevel semantic fusion relation detection model called “MSFR” to boost the performance of critical subtask relation detection in KBQA systems.
* Data
  > 1. Glove [glove.6B.300d.txt] —— Download pre-trained word vectors from <https://nlp.stanford.edu/projects/glove/>
  > 2. All the pre-processed dataset and the trained model can download from https://pan.baidu.com/s/1ErknPmqiGCeBvqvC6N45Mw code: shaf

* Relation Detection Train/Test
  > 1. Run `python main.py -train --data_type sp or python main.py -train --data_type wq` to train the relation detection model.
  > 2. Run `python main.py -test --data_type sp or python main.py -test --data_type wq` to test the relation detection model, and the results saved in ../result/

* Entity Recognition Train/Test
  > 1. Run `python XLNet_NER.py -train or python XLNet_NER.py -train  -wq` to train the entity recognition model.
  > 2. Run `python XLNet_NER.py -test or python XLNet_NER.py -test -wq` to test the entity recognition model, and the results saved in ./result/

* Test our KBQA system
  > 1. Run `python sq_kbqa_system.py` to test our KBQA system on SimpleQuestions.
  > 2. Run `python wq_kbqa_system.py` to test our KBQA system on WebQSP.


References：
1. https://github.com/ypc82/682project
#we will release our code after the paper is accepted.
# msfr
