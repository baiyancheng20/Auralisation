# AuralisationCNN
This repo is for an example of auralisastion of CNNs that is demonstrated on ISMIR 2015.

## Files
auralise.py: includes all required function for deconvolution.
example.py: includes the whole code - just clone and run it by `python example.py`

## Folders
src_songs: includes three songs that I used in my blog posting.

## Usage
Load weights that you want to auralise. I'm using this function
```W = load_weights()```
to load my keras model, it can be anything else.
`W` is a list of weights for the convnet. (TODO: more details)

Then load source files, get STFT of it. I'm using `librosa`.

Then deconve it with `get_deconve_mask`.

## External links
* [The second blog post](https://keunwoochoi.wordpress.com/2016/03/23/what-cnns-see-when-cnns-see-spectrograms/) has more extensive demo. Detailed description will follow after paper submission.
* [The first blog post](http://keunwoochoi.blogspot.co.uk/2015/10/ismir-2015-lbd.html) that explains [my ISMIR 2015 Late-Breaking session paper](http://ismir2015.uma.es/LBD/LBD24.pdf).

#### Credits
* [Keras](https://github.com/fchollet/keras), [librosa](https://bmcfee.github.io/librosa/index.html), [Matt's deconvolution] paper(http://arxiv.org/abs/1311.2901), [Naver Labs](http://labs.naver.com)
