# ChnSetiCorp task
ChnSetiCorp is a dataset for sentiment analysis. 

## Dataset
The corpus can be find [HERE](https://github.com/pengming617/bert_classification)  
Download the corpus and save data at `[ChnSetiCorp_DATA_PATH]`  

## Train and Evaluate
Download ChineseBERT model and save at `[CHINESEBERT_PATH]`.  
Run the following scripts to train and evaluate. 
```
python ChnSetiCorp_train.py \
  --bert_path [CHINESEBERT_PATH] \
  --data_dir [ChnSetiCorp_DATA_PATH] \
  --save_path [OUTPUT_PATH] \
  --max_epoch=10 \
  --lr=2e-5 \
  --warmup_proporation 0.1 \
  --batch_size=8 \
  --weight_decay=0.0001 \
  --gpus="1",
```

## Result
The evaluation metric is **Accuracy**.  
