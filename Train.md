# Creating and Training 
```
cd biaffine-parser-master
```
## Perl Installation

Follow the link for perl installation :
https://linuxhint.com/install-perl-ubuntu/

## conllu_to_conllx.pl

Converts a file in the CoNLL-U format to the old CoNLL-X format.
```
perl conllu_to_conllx.pl < file.conllu > file.conll
```
Move the result .conllx file in <b>data/ptb/</b> folder

## Creating tnt_pos_tagger.dill
```
python3.7 hn_pos.py
```
my_tagger.dill file is created rename it to tnt_pos_tagger.dill and move it to <b>models</b> folder

## Training the model
```
python3.7 run.py train -p --feat=bert --ftrain=data/ptb/tamtrain.conllx --ftest=data/ptb/tamtest.conllx --fdev=data/ptb/tamdev.conllx
```
## Evaluate the model
```
python3.7 run.py evaluate --feat=bert --fdata=data/ptb/tamtest.conllx
```
## Prediction using Web App
Move to the upper directory and then run the web app
```
cd ..
```
```
python3.7 app.py
```
