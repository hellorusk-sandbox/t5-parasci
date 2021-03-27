# t5-parasci

```
python run_paraphrasing.py \
    --model_name_or_path t5-small \
    --seed 42 \
    --do_train \
    --do_eval \
    --do_predict \
    --train_file path_to_csv_or_jsonlines_file \
    --validation_file path_to_csv_or_jsonlines_file \
    --source_prefix "paraphrase: " \
    --output_dir /tmp/tst-paraphrasing \
    --overwrite_output_dir \
    --per_device_train_batch_size=4 \
    --per_device_eval_batch_size=4 \
    --predict_with_generate
```