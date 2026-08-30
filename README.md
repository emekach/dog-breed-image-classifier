# Using a Pre-trained Image Classifier to Identify Dog Breeds

## Project Overview

This project was completed as part of the **Udacity AI Programming with Python Nanodegree**.

The project uses a pre-trained image classifier to identify dogs and classify their breeds from images. Python is used to process the images, obtain expected pet labels, run images through pre-trained CNN models, and evaluate the classification results.

The project also compares the performance of different pre-trained models, including **AlexNet, VGG, and ResNet**.

## Project Goals

The main goals of this project are to:

* Use Python to process a collection of pet images.
* Extract expected pet labels from image filenames.
* Use a pre-trained image classifier to classify images.
* Determine whether the images contain dogs.
* Identify the predicted dog breed.
* Compare predicted labels with the expected labels.
* Calculate classification statistics.
* Compare different pre-trained CNN models.

## Technologies Used

* Python
* PyTorch
* torchvision
* PIL
* NumPy
* Convolutional Neural Networks (CNNs)
* Pre-trained image classification models
* Bash

## Pre-trained Models

Three pre-trained CNN architectures are used in this project:

* **AlexNet**
* **VGG**
* **ResNet**

The models are used to classify the pet images and their performance is compared based on the classification results.

## Project Structure

The project follows the structure provided by the Udacity project:

```text
dog-breed-image-classifier/
│
├── README.md
│
└── data/
    ├── adjust_results4_isadog.py
    ├── calculates_results_stats.py
    ├── check_images.py
    ├── classifier.py
    ├── classify_images.py
    ├── dognames.txt
    ├── get_input_args.py
    ├── get_pet_labels.py
    ├── imagenet1000_clsid_to_human.txt
    ├── print_functions_for_lab_checks.py
    ├── print_results.py
    ├── run_models_batch.sh
    ├── run_models_batch_uploaded.sh
    ├── test_classifier.py
    │
    ├── alexnet_pet-images.txt
    ├── alexnet_uploaded-images.txt
    ├── resnet_pet-images.txt
    ├── resnet_uploaded-images.txt
    ├── vgg_pet-images.txt
    ├── vgg_uploaded-images.txt
    │
    ├── pet_images/
    │   └── ...
    │
    └── uploaded_images/
        └── ...
```

## How the Project Works

### 1. Retrieve Pet Image Labels

The `get_pet_labels.py` program processes the filenames of the pet images and creates a dictionary containing the expected pet labels.

For example:

```text
Golden_retriever_01.jpg
```

can be processed to obtain the expected label:

```text
Golden retriever
```

### 2. Classify the Images

The `classify_images.py` program uses a pre-trained CNN image classifier to classify the images.

The classifier produces a predicted label for each image.

### 3. Determine Whether the Image Contains a Dog

The classifier's predicted label is compared with the list of known dog breeds contained in `dognames.txt`.

This allows the program to determine whether the image is classified as a dog.

### 4. Adjust the Results

The `adjust_results4_isadog.py` program compares the expected pet labels with the classifier predictions and determines whether:

* The expected label is a dog.
* The classifier identified a dog.
* The expected and predicted breeds match.

### 5. Calculate Statistics

The `calculates_results_stats.py` program calculates statistics from the classification results.

These statistics are used to evaluate the performance of the image classifier.

### 6. Print the Results

The `print_results.py` program displays the classification results and statistics in a readable format.

## Model Comparison

The project provides results for:

| Model   | Image Set  |
| ------- | ---------- |
| AlexNet | Pet Images |
| VGG     | Pet Images |
| ResNet  | Pet Images |

The models can be compared based on their ability to correctly identify dogs and classify their breeds.

## Key Learning Outcomes

Through this project, I gained practical experience with:

* Python programming
* Functions and modules
* File handling
* Dictionaries and lists
* String manipulation
* Command-line arguments
* Image classification
* Pre-trained neural networks
* PyTorch
* torchvision
* CNN architectures
* Model evaluation
* Comparing machine learning models

## Running the Project

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/dog-breed-image-classifier.git
```

Navigate into the project:

```bash
cd dog-breed-image-classifier
```

The main project files are located in the `data` directory.

For example:

```bash
cd data
```

The image classification scripts can then be executed using Python and the provided command-line arguments.

## Example

An image such as:

```text
Golden_retriever_01.jpg
```

may produce a result similar to:

```text
Pet Image Label: golden retriever
Classifier Label: golden retriever
Dog: True
Correct Breed: True
```

## Udacity Project

This project was completed as part of the:

**Udacity AI Programming with Python Nanodegree**

The project provided practical experience applying pre-trained image classifiers to a real-world image classification task.

## Author

**Chukwuemeka Chukwuma**

GitHub: **@emekach**

---

This project was completed as part of the **Udacity AI Programming with Python Nanodegree** and is included as part of my machine learning and Python portfolio.

