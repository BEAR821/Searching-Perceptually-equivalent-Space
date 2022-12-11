# Searching-Perceptually-equivalent-Space
Searching Perceptually equivalent Space based on CNN classifier.

You can follow uploaded colab file or ipynb file.

You should download the imagenet dataset from Kaggle.

For our hardware and the size of buffer, we use tiny-imageNet dataset from Kaggle.
(https://www.kaggle.com/datasets/akash2sharma/tiny-imagenet)

And !unzip to unzip the data.

You can easily do experiment by changing hyperparameter.

```
model_name = 'efficientnet_b7' # the name of pre-trained model from torchvision.models

Fix_seed = False # boolean to fix the random seed or not

seed =100 # Set random seed if Fix_seed==False, it gonna ignored

label_size = 50 # N of the report : the number of sampling labels ( for statictical safty )

sample_size = 150 # B of the report : the number of sampling images per label ( for statictical safty )
```

For the analysis, you can load the save data.

```
# root directory of save the result
save_root = ''

Load_result = False

if Load_result:
  load_model = 'efficientnet_b4'
else:
  load_model = model_name # evaluated model

```
