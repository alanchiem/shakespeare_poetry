# shakespeare_poetry

Click [here](https://colab.research.google.com/drive/1Kte1PA77W-47d86fP9K-Jwsll4PPUKIN?usp=sharing) for an interactive version through Google Colab.

or  

[here](https://github.com/alanchiem/shakespeare_poetry/blob/main/Shakespeare_Poetry.ipynb) to view the project on Github.


# My Findings

Each trial was done with 50 epochs.  
Tested by adding 50 additional words after seed text 'to be or not to be.'

Trial Name / Training Accuracy at Epoch 50 / Avg seconds per Epoch

## Trial 1: Shallow and Wide / ~85% / 52s
* Embedding
* Bidirectional LSTM 250
* Dense

Notes: epochs 8 - 12 had a ~10% increase with each epoch. Reached 80% at epoch 18 and stagnated at epoch 25.

*to be or not to be  
alive of me those stars rehearse now shine  
bright dead heart forth me  
now lie in me sad sun is showers new go  
shine bright highmost tomb night memory art more dead 
thee me view new word  
grief thee more delight and date rhyme daily me*  


## Trial 2: Deep and Narrow / ~60% / 24s
* Embedding
* Bidirectional LSTM 50
* Bidirectional LSTM 50
* Dense

Notes: 'room' gets repeated a lot the further from the seed it goes

*to be or not to be  
my love receivest not shine  
thou dumb thereby mind truth hour room grew thou  
no rehearse comment new defaced room room  
bail staineth room room room staineth  
room room bail staineth  
room room room room room pluck crime sad shade like it grace away  
tis extreme grace*  


## Trial 3: Somewhat in the Middle / ~84% / 19s
* Embedding
* Bidirectional LSTM 100
* Dense

Notes: reached 80% at epoch 33

*to be or not to be  
vile delight can prove short  
cold new light decrease light decrease rarities itself  
bastard offenders number in me shall prove new swift dispatch  
dispatch new back vision  
back vision remover doth cures  
be his blood and slave doth stand  
shows you to above the judgment  
part her you dwell bright*
