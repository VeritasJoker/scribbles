
# tigergpu

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

- 20230131-whisper-encoder: whisper-tiny.en en-only onset + ave tokens + layer 0~4 + windows starting from the onset __[Need to adjust for real onset]__
