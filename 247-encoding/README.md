# 247-encoding/data

__brainplot__: electrode coordinates plot, used for Matlab plotting

__podcast_160.csv__: podcast significant electrodes

__podcast-all.csv__: podcast all electrodes

__podcast-old__: old podcast electrode csvs

__tfs-old__: old 247 electrode csvs + some testing for 717 elecs

__tfs-sig-file-old__: *(2022-03)* 247 electrodes based on google significant electrode test

__sig-file-region__: *(2022-09/10)* 247 electrodes based on brain region (potentially handpicked for a grant)

__sig-file-region2__: *(2022-10-25)* 247 electroes baesd on brain region (potentially handpicked for a grant)

__sig-file-brainmap__: *(2022-11-22)* 247 electrodes handpicked for a grant (glove gpt2n-1 gpt2n) + (pred-unpred area)

__tfs-glove-0.08+__: *(2022-11-29)* 247 electrodes based on glove max correlation >= 0.08

__tfs-sig-file-old2__: *(2023-01-09)* 247 electrodes based on google significant electrode test

__20230123-whisper-grant__: 247 electrodes based on whisper vs gpt2n max correlations (handpicked for a grant)



# 247-encoding/results

### 247-bobbi
gpt2 prediction csvs __[for Bobbi]__

### brainplot-20221122
(glove gpt2n gpt2n-1) + 

### brainplot-20230111
(glove gpt2n gpt2n-1) + new sig list

### cor_tfs
(glove gpt bbot)

### cor_tfs-20220123
(glove gpt2n-1 gpt2n) + (area for -500~-100 ms)

### cor_tfs-20220202
(gpt2n-l24 whisper-en-onset-l4) + max cor

### podcast
- podcast-ctx-layer-mwf0: gpt2n-1 + context + layer 1~48
- whisper: encoding on whisper-tiny/base.en embs __[for Aditi]__

### ~~podcast-old~~
- ~~podcast-ctx-layer-mwf0~~
- ~~podcast-ctx-layer-mwf5~~
- podcast-zaid-mwf=0: for Eric's results replication __[for Zaid]__
- podcast-zaid-mwf=5: for Eric's results replication __[for Zaid]__

### podcast-zeroshot [for 0shot paper 1st revision]

### sig_test_new
Trying out some new testing stuff with mixed Gaussian

### tfs

Notes:

__bold__ means a test for important code changes that potentially affect results (every folder ran before __bold__ might be affected)

~~strikethrough~~ means old / not needed / not used results, usually have newer folders with exact same parameters (usually in `tfs-old`)


- __~~20221004-matlab-compare: compare with matlab, bug fixes~~__

- 20221012-glove-concat: glove concat embeddings (up to n + 4) + pca/nopca

- ~~20221024-gpt2~~: (glove + gpt2n + gpt2n-1 + rand + arb) + double lags

- ~~20221101-gpt2-preds~~:
  - ~~(erp + gpt2n + gpt2n-1) + top/bot 0.3 (true_pred_prob)~~ __[token type]__
  - ~~(glove) + top/bot/pred 0.3 (true_pred_prob)~~

- ~~20221102-bert: some bert testing stuff (not sure what exactly)~~

- ~~20221201-gpt2-preds-top5~~: glove + correct/incorrect/pred (rank 5)

- ~~20221205-gpt2-preds-top1~~: glove + correct/incorret/pred (rank 1)

- ~~20230109-gpt2-preds-top5~~: (gpt2n + gpt2n-1) + correct/incorrect (rank 5) __[token type]__

- __~~20230112-token-types: (gpt2n + gpt2n-1) + token types (all/first/last/mean/root)~~__

- ~~20230119-whisper-for-grant~~: whisper-tiny.en + all tokens + layer 0~4 + double lags

- 20230210-798-part-test: test for 798 parts vs convs, test for 798 part preprocessing vs conv preprocessing (waiting for Bobbi on this)

- ~~20230120-whisper-decoder~~: whisper-tiny.en de-only + all tokens + layer 2~3

- ~~20230121-whisper-encoder~~: whisper-tiny.en en-only + all tokens + layer 1~4

- ~~20230127-whisper-encoder-offset~~: whisper-tiny.en en-only offset + ave tokens + layer 0~4 + windows 1/2/3/4/5/6/1~3/1~6/1~9/1~12 starting from the offset

- ~~20230130-whisper-encoder-onset~~: whisper-tiny.en en-only onset + ave tokens + layer 0~4 + windows 0.5/1/2.5/3/5 starting from the offset

- ~~20230131-whisper-encoder-onset~~: whisper-tiny.en en-only onset + ave tokens + layer 0~4 + windows starting from the onset __[Grant results, but need to adjust for real onset]__

- 20230210-whisper-encoder-onset: whisper-tiny.en en-only onset + ave tokens + layer 0~4 + windows starting from the onset

- 20230212-whisper-decoder: whisper-tiny.en de-only + ave tokens + layer 0~4

- ~~20230214-gpt2-preds~~: (gpt2n + gpt2n-1) + correct/incorrect (rank 5) + top/bot (0.3)

- ~~20230214-gpt2-preds-della~~: (gpt2n + gpt2n-1) + correct/incorrect (rank 1)

- 20230216-whisper-full: whisper-tiny.en + ave tokens + layer 0~4 (n-audio)

- 20230219-gpt2-layers: testing gpt2 layers for 247 grant (rough scan by 5)

- __20230220-xtraf-test: testing if xtraf makes a difference__ __[Sadly it does, everything needs to rerun]__

- 20230221-pred-diffs: difference in prediction * (glove + gpt2n + gpt2n-1) + (rank 5 + rank 1 + pred 0.3)

- 20230225-gpt2-layers: testing gpt2 layers for 247 grant (some tokens wrongly deleted because aligning with gpt2-xl) (need 717 and 798 embedding regeneration)

- 20230226-gpt2-preds: final 247 results for all preds (gpt2n + gpt2n-1)

- 20230227-gpt2-preds: final 247 results for all preds (glove + gpt2 aligned)

- 20230228-all-embs: final 247 results for 20221024-gpt2 (will also add 20221012-glove-concat)

- 20230303-whisper-preds: whisper decoder preds (preliminary results, Leo will rerun everything for whisper)


### uriplot2
(glove gpt2n gpt2n-1) + (all pred unpred) + (different brain regions)