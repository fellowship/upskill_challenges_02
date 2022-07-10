# No-code Platform Challenges
Platform Challenges are non-coding Machine Learning challenges. You are expected to create a training dataset, train and test your models, then send your model along with their predictions. The Challenges are:
- **Jeans Challenge**
- **Jackets and Shirt Challenge**


## Jeans Challenge

Your goal for this challenge is to train a machine learning model to classify images of Levi's jeans according to fit, and then use that trained model to predict fits for randomized jean images: 

![Image Classification Diagram](https://github.com/fellowship/upskill_challenges_02/blob/main/imgs/cv_model_diagram.png)

The challenge has three main steps:

1. Build a training data set of jean images.
2. Train a Computer Vision model using your data set.
3. Use your trained model to classify images of Levi's jeans according to fit.

Use [Lobe.ai](https://lobe.ai/) to complete this challenge. Lobe is a no-code machine learning platform you can use to label data, train models, and make predictions without any prior code or machine learning knowledge. Refer to the [website](https://lobe.ai/) for more information on how to use the product.

### Instructions

You need to download and install Lobe to your local system to complete this challenge. LS&Co. has issued specific instructions on how to do so for Levi's issued computers. Refer to the instructions for [installing Lobe on Mac](https://github.com/fellowship/upskill_challenges_02/blob/main/Platform/installation/Install%20Lobe%20on%20Mac.pdf) or [installing Lobe on Windows](https://github.com/fellowship/upskill_challenges_02/blob/main/Platform/installation/Install%20Lobe%20Windows.pdf) to get the software downloaded and installed on your machine.

In the [data repository](https://github.com/fellowship/upskill_challenges_02/blob/main/Platform/Data/jeans_challenge_data.zip) you'll find a dataset of 40 randomized jean images. Each of the jeans belongs to one of four fits:

- **Men 501**
- **Men 550**
- **Women 501** 
- **Women 711**

Your goal for this challenge is to train and use a model to predict which fit each randomized image belongs to. The model must predict exactly one of the following labels for each image: 

- **m_501**
- **m_550**
- **w_501**
- **w_711**

Start by building a data set of training images from the web. Your dataset will have to include images from each of the 4 styles, and can't include any of the 40 images from the challenge data. While building your dataset make sure you re-name the images to reflect the fit and image number: m_501_1.jpg, m_501_2.jpg, etc. 

_Hint: the 40 images in the challenge data were scraped from the Levi's website; you may need to look elsewhere for some your data._

Once you have your data organized, named, and numbered you should use Lobe to assign machine learning labels to each image: m_501, w_501, etc. With labeled data in Lobe you can train the model and use it to predict a fit for all the images in the challenge data.

### Guidelines

- None of the randomized images from the challenge data should be in your data (that's data leakage!)
- Your training data should contain fewer images than the challenge data set (<40 images).
- The training data should be as small as possible, i.e. you want to maximize the performance of the model while using the smallest possible training data set.
- Image labels in Lobe must exactly match one of the following: m_501, m_550, w_501, w_711.
- Don't hand-label the challenge images: you must use a model to predict the fit.
- Make sure you're capable of discussing your methodology and solution during an interview.

### Deliverables

Your submission should be a single zip file containing the following:

- Your predictions for the jean images: A CSV file containing the image file names and the corresponding predictions. The CSV file should be named _**yourfirstname_yourlastname_predictions.csv**_ and have the following format when viewed in Excel:

| file_name        | prediction |
|------------------|------------|
| 1kDc10mxMfle.jpg | m_501      |
| 5NtNguD8pCKo.jpg | w_711      |

-Note:_Lobe might not export the csv, you will have to fill a Excel file manually, then save as csv_

- Your training data: The training data set you used to train your model, including image labels as file names, in a folder named _**yourfirstname_yourlastname_training_data.**_

Put your CSV file and the folder with the training data into a folder named _**yourfirstname_yourlastname_platform_jeans,**_ compress the folder, and upload the zip file to OneDrive, Google Drive, or DropBox. [Log in](https://www.launchpad.ai/upskill/levis/login) to your account and upload the public file sharing link via the dashboard.

## Jackets and Shirts Challenge
Similar to the jeans challenge,  your goal for this challenge is to train a machine learning model to classify images of Levi's jackets and shirts, and then use the trained model to make predictions on the test set of randomized images: 

In the [data repository](https://github.com/fellowship/upskill_challenges_02/blob/main/Platform/Data/jackets_challenge_data.zip) you'll find a dataset of 30 randomized images. Each of the images belongs to one of three labels:
- **Puffer Jackets**
- **Trucker Jackets**
- **Shirts** 


Your model should predict labels as follows:
- **Puffer**
- **Trucker**
- **Shirt**


### Instructions
-  Build a dataset of training images from the web. 
-  Rename your training images according to their label, example: Puffer_1.jpg, Puffer_2.jpg, Trucker_1.jpg, etc
-  The images for training should not include any image from the testset. 
-  Training dataset should be 30 images in total, 10 images per class.

### Deliverables

Your submission should be a single zip file containing the following:

- Your **predictions** for test images: A CSV file containing the image file names and the corresponding predictions. The CSV file should be named
- **yourfirstname_yourlastname_predictions.csv**_ and have the following format when viewed in Excel:

| file_name        | prediction |
|------------------|------------|
| 1kDc10mxMfle.jpg | Puffer     |
| 5NtNguD8pCKo.jpg | Trucker     |


- Your **training data**: The training data set you used to train your model, including image labels as file names, in a folder named _**yourfirstname_yourlastname_training_data.**_

Put your CSV file and the folder with the training data into a folder named _**yourfirstname_yourlastname_platform_jackets,**_ compress the folder, and upload the zip file to OneDrive, Google Drive, or DropBox. [Log in](https://www.launchpad.ai/upskill/levis/login) to your account and upload the public file sharing link via the dashboard.

## Deadline
[Log in](https://www.launchpad.ai/upskill/levis/login) to your account and upload the public file sharing link via the dashboard. Don't put your file in a folder before compressing; compress the file itself. Challenges should be submitted no later than midnight PST on **August 25** for all employees.
