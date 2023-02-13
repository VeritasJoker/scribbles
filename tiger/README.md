# 247-encoding/data

### brainplot
electrode coordinates plot, used for Matlab plotting

### podcast_160.csv
podcast significant electrodes

### podcast-all.csv
podcast all electrodes

### podcast-old
old podcast electrode csvs

### sig-file-brainmap (2022-11-22)
247 electrodes handpicked for a grant (glove gpt2n-1 gpt2n) + (pred-unpred area)

### sig-file-region (2022-09/10)
247 electrodes based on brain region (potentially handpicked for a grant)

### sig-file-region2 (2022-10-25)
247 electroes baesd on brain region (potentially handpicked for a grant)

### 20230123-whisper-grant
247 electrodes based on whisper vs gpt2n max correlations (handpicked for a grant)

### tfs-glove-0.08+ (2022-11-29)
247 electrodes based on glove max correlation >= 0.08

### tfs-sig-file-old (2022-03)
247 electrodes based on google significant electrode test

### tfs-sig-file-old2 (2023-01-09)
247 electrodes based on google significant electrode test




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
- __20221004-matlab-compare: compare with matlab, bug fixes__

- 20221012-glove-concat: glove concat embeddings (up to n + 4) + pca/nopca

- 20221024-gpt2: (glove + gpt2n + gpt2n-1 + rand + arb) + double lags

- 20221101-gpt2-preds:
  - ~~(erp + gpt2n + gpt2n-1) + top/bot 0.3 (true_pred_prob)~~ __[token type]__
  - (glove) + top/bot/pred 0.3 (true_pred_prob)

- 20221201-gpt2-preds-top5: glove + correct/incorrct/pred (rank 5)

- 20221205-gpt2-preds-top1: glove + correct/incorret/pred (rank 1)

- ~~20230109-gpt2-preds-top5~~: (gpt2n + gpt2n-1) + correct/incorrect (rank 5) __[token type]__

- __20230112-token-types: (gpt2n + gpt2n-1) + token types (all/first/last/mean/root)__

- ~~20230119-whisper-for-grant~~: whisper-tiny.en + all tokens + layer 0~4 + double lags

- ~~20230120-whisper-decoder~~: whisper-tiny.en de-only + all tokens + layer 2~3

- ~~20230121-whisper-encoder~~: whisper-tiny.en en-only + all tokens + layer 1~4

- ~~20230127-whisper-encoder-offset~~: whisper-tiny.en en-only offset + ave tokens + layer 0~4 + windows 1/2/3/4/5/6/1~3/1~6/1~9/1~12 starting from the offset

- ~~20230130-whisper-encoder-onset~~: whisper-tiny.en en-only onset + ave tokens + layer 0~4 + windows 0.5/1/2.5/3/5 starting from the offset

- ~~20230131-whisper-encoder-onset~~: whisper-tiny.en en-only onset + ave tokens + layer 0~4 + windows starting from the onset __[Grant results, but need to adjust for real onset]__

- 20230210-whisper-encoder-onset: whisper-tiny.en en-only onset + ave tokens + layer 0~4 + windows starting from the onset

- 20230212-whisper-decoder: whisper-tiny.en de-only + ave tokens + layer 0~4


### uriplot2
(glove gpt2n gpt2n-1) + (all pred unpred) + (different brain regions)