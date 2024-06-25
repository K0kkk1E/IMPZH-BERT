# THUCNews task
THUCNews is a dataset for document classification task. 

## Dataset
The corpus can be find [HERE](https://github.com/gaussic/text-classification-cnn-rnn)  
Download the corpus and save data at `[THUCNews_DATA_PATH]`  

## Train and Evaluate
Download ChineseBERT model and save at `[CHINESEBERT_PATH]`.  
THUCNews is a classification task with ten classes, so you have to
modify `[CHINESEBERT_PATH]/config.json` file, and set `"num_labels":10`.
Run the following scripts to train and evaluate. 

```bash
python THUCNews_train.py --bert_path "[CHINESEBERT_PATH]" --data_dir "[THUCNews_DATA_PATH]" --save_path "[OUTPUT_PATH]" --max_epoch=5 --lr=2e-5 --batch_size=4 --gpus="1"
```

## Result
The evaluation metric is **Accuracy**.  
