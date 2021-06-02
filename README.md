# Dutch Kaldi Profile

A [Rhasspy](https://github.com/rhasspy/rhasspy) profile for Dutch (`nl`).

Includes:

* A [Kaldi nnet3](https://kaldi-asr.org/doc/dnn3.html) speech to text model
    * See files in `acoustic_model/`
    * Recipe created with [ipa2kaldi](https://github.com/rhasspy/ipa2kaldi)
    * Word error rate: 14.29%
    * Trained on:
        * [MLS](http://openslr.org/94/) (1,579 hours)
        * [CGN](http://lands.let.ru.nl/cgn/ehome.htm) (314 hours)
        * [Common Voice](https://commonvoice.mozilla.org) (63 hours)
        * [Voxforge](http://voxforge.org/nl) (10 hours)
* An [IPA](https://en.wikipedia.org/wiki/International_Phonetic_Alphabet) pronunciation lexicon
    * See `base_dictionary.txt.gz`
* A [phonetisaurus](https://github.com/AdolfVonKleist/Phonetisaurus) grapheme to phoneme model for predicting word pronunciations
    * See `g2p.fst.gz`
    * Trained on `base_dictionary.txt.gz`
* A tri-gram [ARPA language model](https://cmusphinx.github.io/wiki/arpaformat/)
    * See `base_language_model.txt.gz`
    * Text from audio transcriptions, [Common Voice](https://github.com/mozilla/common-voice/tree/master/server/data/nl), and [Universal Dependencies](https://universaldependencies.org/)
