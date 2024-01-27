# Dependency-parser
## Dependencies :
* OS : Ubuntu 22.04.3 LTS
* Python 3.7
* flask 1.1.1
* flask-wtf 0.14.2
* flask-markdown 0.3
* nltk 3.4.5
* pygraphviz 1.7
* conllu 2.2.2
* scikit-learn 0.22.1
* dill 0.3.1.1
* transformers 2.1.1

```bash
> python3.7 -m pip install torch==1.7.1+cu110 torchvision==0.8.2+cu110 torchaudio==0.7.2 -f https://download.pytorch.org/whl/torch_stable.html
```

## Instructions for web app :

Run the following to host the app at localhost:5000
```bash
> python3.7 app.py
```
## Results :
Trained a model using <b>BERT</b> and parser implemented from <b>Deep Biaffine Attention for Neural Dependency Parsing</b> on Telugu UD Treebank dataset

<b>
train: 400  sentences
</b>
<br>

<b>
dev:     80 sentences
</b>
<br>

<b>
test:    120 sentences
</b>


### Train
Training the model

![parameter](https://github.com/varunlmxd/Dependency-Parser/assets/104298930/304c0f93-a377-4a9f-a9cd-34f9d756ba3a)

### Evaluate

Evaluation score after testing with Test Dataset

![evaluate](https://github.com/varunlmxd/Dependency-Parser/assets/104298930/5c245c8a-2fe6-4e6a-b3f1-63b5503b8140)
### Prediction


#### Entering the sentence

![before](https://github.com/varunlmxd/Dependency-Parser/assets/104298930/9c725d7e-40d9-4caf-8666-86bf4dc06419)

#### Final Result

![finalres](https://github.com/varunlmxd/Dependency-Parser/assets/104298930/d6cd1260-3e8d-4352-96f6-97061a829d58)

#### Original Values

![original](https://github.com/varunlmxd/Dependency-Parser/assets/104298930/84391246-41f5-469d-90f9-d86e18494999)

