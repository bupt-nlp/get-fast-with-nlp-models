# get-fast-with-nlp-models
we define the standard and common dataprocess module and code to improve the process coding nlp models.

## Features

- define the input & output of the model, so all of you should do is to write your model code.
- supply the common tools that you need in your projects.
- 

## sequence-labeling models


### All of things you should do

- Install

```shell
pip install -r requirements.txt
```

- Process your data to the file format

> this is the sequence labeling task model, so if you process your data to the file format, you can fed the file to our model at free. And the model will return the specific format file to you. The following is the format of the input file

```shell
token1 token2 token3 ... tokenn\tlabel1 label2 label3 ... labeln
```

- Complete configuration

```shell
python main.py \
    --do_train=True \
    --do_eval=True \
    --do_predict=True \
    --input_file=data.train \
    --output_file=data.train.result \
    --batch_size=10 \
    --lr=5e-5 \
    --hidden_size=768 \
```