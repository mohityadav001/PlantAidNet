### Details About the code

- The .ipynb file contains the complete code from loading the images to training,evaluation and prediction of the model.<br/>
- The code has has been written using PyTorch framework.

### List of Plants and Diseases that the model can detect

#### Unique Plants:

Pepper, Grape, Tomato, Squash, Corn, Apple, Potato, Raspberry, Strawberry, Cherry, Soybean, Blueberry, Orange, Peach

#### List of Diseases:

- 'Apple**_Apple_scab', 'Apple_**Black_rot', 'Apple**_Cedar_apple_rust', 'Apple_**healthy'
- 'Blueberry\_\_\_healthy'
- 'Cherry\_(including_sour)**_Powdery_mildew', 'Cherry_(including*sour)***healthy'
- 'Corn\_(maize)**_Cercospora_leaf_spot Gray_leaf_spot', 'Corn_(maize)\_**Common*rust*', 'Corn\_(maize)**_Northern_Leaf_Blight','Corn_(maize)\_**healthy',
- 'Grape**_Black_rot', 'Grape_**Esca\_(Black_Measles)', 'Grape**_Leaf_blight_(Isariopsis*Leaf_Spot)', 'Grape***healthy'
- 'Orange*\_\_Haunglongbing*(Citrus_greening)'
- 'Peach**_Bacterial_spot', 'Peach_**healthy'
- 'Pepper,\_bell**_Bacterial_spot', 'Pepper,\_bell_**healthy',
- 'Potato**_Early_blight', 'Potato_**Late_blight', 'Potato\_\_\_healthy'
- 'Raspberry\_\_\_healthy'
- 'Soybean\_\_\_healthy'
- 'Squash\_\_\_Powdery_mildew'
- 'Strawberry**_Leaf_scorch', 'Strawberry_**healthy',
- 'Tomato**_Bacterial_spot', 'Tomato_**Early_blight', 'Tomato**_Late_blight', 'Tomato_**Leaf_Mold','Tomato**_Septoria_leaf_spot', 'Tomato_**Spider_mites Two-spotted_spider_mite', 'Tomato**_Target_Spot', 'Tomato_**Tomato_Yellow_Leaf_Curl_Virus', 'Tomato**_Tomato_mosaic_virus', 'Tomato_**healthy'

#### Workflow of Code:

1. Loading the images from the folder resizing them into 128 _ 128 (256 _ 256 takes time for processing) and coverting them to tensors
2. Building a validation dataset using 0.3% of the total dataset.
3. Loading the data using Batches
4. Trying various CNN architecture

- Combination of Multilayer CNN with Linear Layers
- VGG16 using Transfer Learning
- Resnet34 using Transfer Learning

5. Selecting the device and loading the data into device i.e (GPU)
6. Training the model and evaluating the model on test data
7. Saving the Model
