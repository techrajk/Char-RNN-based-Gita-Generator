## Bhagvad Gita generator using Char-RNN
 
This is a fun project to generate verses of **BHAGVAD GITA** using Multi-layer Recurrent Neural Networks (LSTM, RNN) for character-level language models in Python using Tensorflow.

Inspired from Andrej Karpathy's [char-rnn](https://github.com/karpathy/char-rnn).

## Usage
To train with default parameters on the text corpus, run `python train.py`. To access all the parameters use `python train.py --help`.

To sample from a checkpointed model, `python sample.py`.
Sampling while the learning is still in progress (to check last checkpoint) works only in CPU or using another GPU.
To force CPU mode, use `export CUDA_VISIBLE_DEVICES=""` and `unset CUDA_VISIBLE_DEVICES` afterward
(resp. `set CUDA_VISIBLE_DEVICES=""` and `set CUDA_VISIBLE_DEVICES=` on Windows).

To continue training after interruption or to run on more epochs, `python train.py --init_from=save`

## Dataset
To avoid copyright issues Bhagvad Gita in txt format is not provided.You may source a copy of it from somewhere and put it in data/bhagavad-gita/ folder and rename it as 'input.txt' to run it from scratch.Otherwise, you may use checkpoints saved under save folder and run for few more epochs for better results.

### Disclaimer
This is just a project to understand/demonstarte NLP and TF concepts and not intended for any copyright infringement or hurting religious sentiments.If you have any objection feel free to mail me.     

## Credits
The code for this project is borrowed from this git repo [sherjilozair/char-rnn-tensorflow]https://github.com/sherjilozair/char-rnn-tensorflow.

