# 0shot-pickling
`results/podcast/777/pickles/pickles` is the old folder with all the old files, with `777_full_labels_fold.pkl` being the fold label pickle used in embedding generation inside each fold and `777_binned_signal_200.pkl` being the newly generated pickle with `200 ms` bins (copied from `pickles2` folder).

`results/podcast/777/pickles/pickles2` is the new folder generated with the newest version of `247-pickling`. Everything is generated with `200 ms` bins, although it should only affect the binned signal pickle.


# 0shot-encoding

`results/podcast/*-glove50` is the glove encoding results generated during 1st revision, correspond to `resultfs/figures/glove`

`results/podcast/*-gpt2-xl` is the gpt2 encoding results generated during 1st revision, correspond to `resultfs/figures/gpt2`

`results/podcast/*-gpt2-xl-fold` is the gpt2 encoding results generated during 2st revision (within-fold embeddings), correspond to `resultfs/figures/gpt2-fold`

`results/podcast/*-gpt2-xl-fold-2` is the gpt2 encoding results generated during 2st revision (within-fold embeddings) (aligned with glove50), correspond to `resultfs/figures/gpt2-fold-aligned`

`results/podcast/*-glove50-concat10` is the glove encoding results generated during 2st revision (concatenation of previous 10 embeddings), correspond to `resultfs/figures/glove-concat`

`results/podcast/*-glove50-concat10-2` is the glove encoding results generated during 2st revision (concatenation of previous 10 embeddings) (no leakage between folds) (aligned with gpt2), correspond to `resultfs/figures/glove-concat-aligned`

`results/podcast/*-glove50-concat10-3` is the glove encoding results generated during 2st revision (concatenation of previous 10 embeddings) (no leakage between folds) (aligned with gpt2) (near neighbor on PCA), correspond to `resultfs/figures/glove-concat-aligned`



# 0shot-decoding

Any folder ending with `0`: not sure what those are (same args as `2`s?)

Any folder ending with `2`: replication of original results

Any folder ending with `3`: within-fold embeddings


