# vivid123


## Run single generation task
```bash
python run_generation.py
```

## Prepare batch generation config yaml file
```bash
python -m scripts.job_config_yaml_generation 
```
This will put all the yaml files in the `tasks` folder.

## Run batch generation tasks
```bash
CUDA_VISIBLE_DEVICES=0 python run_batch_generation.py --configs_dir=tasks --dataset_dir=gso-rendered-reference-45-starting-0-ending-90 --output_dir=outputs --obj_csv_file=scripts/gso_metadata_object_prompt_100.csv --run_from_obj_index=0 --run_to_obj_index=50
```
