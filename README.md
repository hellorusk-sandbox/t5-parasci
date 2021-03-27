# t5-parasci

```
CUDA_VISIBLE_DEVICES=* poetry run python run_paraphrasing.py \
    --model_name_or_path t5-base \
    --seed 42 \
    --do_train \
    --do_eval \
    --do_predict \
    --train_file ParaSCI-ACL/train.csv \
    --validation_file ParaSCI-ACL/validation.csv \
    --test_file ParaSCI-ACL/test.csv \
    --source_prefix "paraphrase: " \
    --output_dir output \
    --overwrite_output_dir \
    --per_device_train_batch_size=16 \
    --per_device_eval_batch_size=16 \
    --num_train_epochs 10 \
    --predict_with_generate \
    --max_source_length 128 \
    --max_target_length 128
```

not overwrite

```
CUDA_VISIBLE_DEVICES=* poetry run python run_paraphrasing.py \
    --model_name_or_path t5-base \
    --seed 42 \
    --do_train \
    --do_eval \
    --do_predict \
    --train_file ParaSCI-ACL/train.csv \
    --validation_file ParaSCI-ACL/validation.csv \
    --test_file ParaSCI-ACL/test.csv \
    --source_prefix "paraphrase: " \
    --output_dir output \
    --per_device_train_batch_size=16 \
    --per_device_eval_batch_size=16 \
    --num_train_epochs 10 \
    --predict_with_generate \
    --max_source_length 128 \
    --max_target_length 128
```