# Food-Prediction-WebApp-using-Tensorflow :hamburger: :camera:

We have built an end-to-end **CNN Image Classification Model** which identifies the food in your image. 

I worked out with a pre-trained Image Classification Model that comes with Keras and then retrained it on the infamous **Food101** Dataset.

### Fun Fact 

The Model actually beats the [**DeepFood**](https://arxiv.org/pdf/1606.05675.pdf) Paper's model which also trained on the same dataset.

The Accuracy aquired by DeepFood was **77.4%** and our model's **85%** . Difference of **8%** ain't much, but the interesting thing is, DeepFood's model took **2-3 days** to train while our's barely took **90min**.

> ##### **Dataset used :**  **`Food101`**

> ##### **Model Used :** **`EfficientNetB1`**

> ##### **Accuracy :** **`85%`**

## Looks Great, How can I use it ?

Finally after training the model, I have exported it as `.hdf5` files and then integrated it with **Streamlit Web App**. 

**Streamlit** turns data scripts into shareable web apps in minutes. 

### Check the demo video



https://github.com/HiteshRam666/Food-Prediction-WebApp-using-Tensorflow/assets/116026459/60cb21ea-ff45-4e38-a4cf-8246a5a776a5


https://github.com/HiteshRam666/Food-Prediction-WebApp-using-Tensorflow/assets/116026459/8e9125db-5a46-4877-a2d4-7e0f81f44304


https://github.com/HiteshRam666/Food-Prediction-WebApp-using-Tensorflow/assets/116026459/fe58992b-34bd-42fd-a355-c946162daa5c





Once an app is loaded, 

1. Upload an image of food. If you dont have one, use the images from `food-images/`
2. Once the image is processed, **`Predict`** button appears. Click it.
3. Once you click the **`Predict`** button, the model prediction takes place and the output will be displayed along with the model's **Top-5 Predictions**
4. And voilà, there you go.

## Breaking down the repo

At first glance the files in the repo may look intimidating and overwhelming. To avoid that, here is a quick guide :

* `.gitignore` : tells what files/folders to ignore when committing
* `app.py`  : Our Food Vision app built using Streamlit
* `utils.py`  : Some of used fuctions in  `app.py`
* `model-training.ipynb`  : Google Colab Notebook used to train the model
* `model/`  : Contains all the models used as *.hfd5* files
* `requirements.txt`  : List of required dependencies required to run `app.py`
* `extras/`  : Has some miscellaneous images and files used to write this README Document

