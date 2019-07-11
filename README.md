# MusicGen
Generate music using Character Wise Recurrent Neural Network


## Dataset
The dataset used here is the ABC music files from [Nottingham Music Database](http://abc.sourceforge.net/NMD/) .

#### ABC music notation
In the abc notation the music file looks something like this:

X:1

T:Speed the Plough

M:4/4

C:Trad.

K:G

|:GABc dedB|dedB dedB|c2ec B2dB|c2A2 A2BA|

  GABc dedB|dedB dedB|c2ec B2dB|A2F2 G4:|
  
|:g2gf gdBd|g2f2 e2d2|c2ec B2dB|c2A2 A2df|

  g2gf g2Bd|g2f2 e2d2|c2ec B2dB|A2F2 G4:|
  
## Requirements
* Tensorflow
* Numpy
* TQDM
* Glob
* abc2midi Converter

## Char RNN

This is how the character wise RNN looks like.
![alt text](https://github.com/nj2610/MusicGen/blob/master/assets/charRNN%400.5x.png "Char RNN")

The detailed description is provided in the notebook itself.

## Output
The code outputs a sequence of characters that will be the abc notation of the music generated. After that we have to use a abc to midi converter
to get the output music.
