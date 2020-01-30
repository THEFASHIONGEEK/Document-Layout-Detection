# Document Layout Detection


![Document Layout Detection](Images/Layout_Analysis.png)


## Pipeline

Run the requirements.txt 

```
pip install -r requirements.txt
```


```
gtf.Train_Dataset(root_dir="../sample_dataset", coco_dir="kangaroo", img_dir="images", set_dir="Train", batch_size=8, image_size=512, use_gpu=True)
```
Load Model

```
gtf.Model()
```
Set Hyper Parameters

```
gtf.Set_Hyperparams(lr=0.0001, val_interval=1, es_min_delta=0.0, es_patience=0)
```

Start the training 

```
gtf.Train(num_epochs=2, model_output_dir="trained/")
```



## Acknowledgments

* [MONK_OBJECT_DETECTION](https://github.com/Tessellate-Imaging/Monk_Object_Detection)
