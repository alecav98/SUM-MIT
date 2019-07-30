# SUM+MIT
​
SUM+MIT is a tool created in Google Colaboratory (Colab) that can solve a mathematics equation using image classification.
​
The motivation behind this project was a personal one. Our team wanted to apply data and image preprocessing, object detection, and image classification on multiple digits and symbols.
​
## Datasets Used
​
We used the [MNIST dataset](https://www.kaggle.com/rakuraku678/mnist-60000-hand-written-number-images) for digits, and a [Kaggle dataset](https://www.kaggle.com/xainano/handwrittenmathsymbols) for symbols. The MNIST dataset contained 70,000 images of white digits written on a black background. The Symbols dataset contained 100,000 images of 82 different math symbols and the numbers 0 through 9.
​
It should be noted that the Symbols dataset contained pixel-by-pixel duplicated images which we removed. Thus, we ended up with ~82,000 symbols images.
​
## Getting Started
​
These instructions will get you a copy of the project up and running on your own Colab notebook.
​
The data preprocessing notebook, "Preprocessing1.ipynb", takes the MNIST Digits dataset and the Symbols dataset and converts them into two csv files. These two files, "inverted_df" and "inverted_test_df" are the training and testing csv files that are used in the "FinalCopy.ipynb".
​
There are three preprocessing notebooks, they must be ran in order (1,2,3) because every notebook uses files generated in the notebook before it. The first notebook takes the MNIST Digits dataset and prepares it for merging with the symbols dataset. Similarly, the second notebook prepares the Symbols dataset. Finally, the third preprocessing notebook merges both datasets and finishes preparing the merged dataset so that it is compatible with the model.
​
You could run "Preprocessing1.ipynb", "Preprocessing2.ipynb", "Preprocessing3.ipynb" to generate both 'inverted_df' and 'inverted_test_df' or you could use the copies we provided in this repo to simply run "Model.ipynb".
​
You can download the notebook to your personal computer, simply make sure that you have all the necessary imports before running the code. Once you are in your copy, you can navigate to the left side of the page and open the Files tab. Here, you can upload any files necessary to run the notebook.
​
## Using SUM+MIT
​
In order to use SUM+MIT, create your own copy of "Model.ipynb" and upload the necessary files. Then, follow the code. The section entitled "Upload your equation" will open up a camera in Colab, where you will be able to take a picture of your own equation.
​
Continue following the code to the end, where you will arrive at your solution.
​
## Built With
​
* [Google Colaboratory](https://colab.research.google.com/notebooks/welcome.ipynb) - The Jupyter notebook environment used
* [Python and supported libraries](https://www.python.org/) - The programming language used
* [TensorFlow](https://www.tensorflow.org/) - The core open source library to develop and train our ML model
* [OpenCV](https://opencv.org/) - The library of computer vision programming functions used
* [Keras](https://keras.io/) - A high-level neural networks API used
​
## Authors
​
* **Lizzet Clifton**
* **Alejandro Caviedes**
* **Christopher O'Rourke**
* **Rosemary Austin**
​
## Acknowledgments
​
* Big thanks to Google's Applied Machine Learning Intensive!
