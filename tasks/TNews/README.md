# TNews task 
TNEWS is a 15-class short news text classification dataset. <br>

## Dataset
The official TNEWS corpus can be find [HERE](https://storage.googleapis.com/cluebenchmark/tasks/tnews_public.zip)  
Download the corpus and save data at `[TNEWS_DATA_PATH]`


## Train and Evaluate
Download ChineseBERT model and save at `[CHINESEBERT_PATH]`.  
Run the following scripts to train and evaluate on the validation set. 
If you would like to evaluate the model on the test set, please submit the model prediction to [CLUE](https://www.cluebenchmarks.com/)

```bash
python TNews_train.py --lr 3e-5 --max_epochs 10 --max_length 256 --weight_decay 0.002 --hidden_dropout_prob 0.2 --warmup_proportion 0.02 --batch_size 16 --accumulate_grad_batches 1 --save_topk 20 --val_check_interval 0.25 --bert_path "[CHINESEBERT_PATH]" --data_dir "[TNEWS_DATA_PATH]" --save_path "[OUTPUT_PATH]" --gpus="1" --precision=16
```

## Result
The evaluation metric is **Accuracy**.  
