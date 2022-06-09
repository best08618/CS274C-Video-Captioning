# CS274C-Video-Captioning

We implement Baseline model and attention model with Keras. 
Below is the steps for preprocessing data and training/ testing.

All the video files should be in a right directory (training_data/video/)

```
You can use the trained-models for experiments.
model_final2022-06-02.tar.gz # baseline model
model_att_general_2022-06-02.tar.gz #attention model 
```


## 01. Feature Extractor
We need to preprocess each video and extract features from the video using pre-trained model.

Run this jupyter notebook. 
It will preprocess all the videos in "training_data/video" folder and save feature as .npy file to "training_data/features_dir"

```
Feature_Extractor.ipynb 

```

## 02. Baseline Model
For the training and testing baseline model (simple seq2seq), run below jupyter notebook.
```
Video captioning_baseline.ipynb 

```

This will train the model and save the model and if you run the inference code, it will generate caption for the test dataset.

## 03. Attention Model
For the training attention model, run below jupyter notebook.
```
[Training] Video captioning_attention.ipynb

```

For getting inference from the attention model, run below jupyter notebook.
```
[Inference] Video captioning_attention.ipynb
```

## 04. Evaluate Model
For evaluating the generation from each model, run below jupyter notebook.
```
evaluation.ipynb
```
Just set the file path as the inference result file from the model that you want to evaluate.

