# Universal Dependencies for Tweets in Brazilian Portuguese: Tokenization and Part of Speech Tagging
This repository contains additional resources for the paper "Universal Dependencies for Tweets in Brazilian Portuguese: Tokenization and Part of Speech Tagging" to be published in ENIAC 2021.

We used a modified version of [UDPipe 1](https://github.com/huberemanuel/udpipe/tree/tagger_only), where we removed the parsing and tokenization components.

For UDPipe 2, we used the original repository located at [here](https://github.com/ufal/udpipe/tree/udpipe-2).

In [Udify](https://github.com/huberemanuel/udify), we had to patch an update enabling the reading of treebanks without dependency relations. This is due to DANTE being under construction. Although, you should be able to use the original [repo](https://github.com/Hyperparticle/udify) if your treebank has the dependency relations labels.

We evaluated model results with this [script](https://github.com/huberemanuel/udpipe/blob/udpipe-2/udpipe2_eval.py). You should be able to run it with the following command:

```bash
python3 udpipe2_eval.py gold_file.conllu pred_file.conllu --verbose
```

The confusion matrices for the final training is available in the `assets` folder.