# Kaggle Datathon IBM WIDS 2019
Predict Palm Oil plantation using satellite images for deforestation affects.

Link to Competition : https://www.kaggle.com/c/widsdatathon2019

Secured #81 Rank on Public Dataset
The challenge was to create a model that predicts the presence of oil palm plantations in satellite imagery. Planet and Figure Eight have generously provided an annotated dataset of satellite images recently taken by Planet satellites. 

The dataset images are 3-meter spatial resolution, and each is labeled with whether an oil palm plantation appears in the image (0 for no plantation, 1 for any presence of a plantation).

The datathon task was to train a model that takes as input a satellite image and outputs a prediction of how likely it is that the image contains an oil palm plantation. Labeled training and test datasets are provided for model development


# Why oil palm?

Deforestation through oil palm plantation growth represents an agricultural trend with large economic and environmental impacts. From shampoo to donuts and ice cream, oil palm is present in many everyday products—but many have never heard of it explicitly! Because oil palm grows only in tropical environments, the crop’s expansion has led to deforestation, increased carbon emissions, and biodiversity loss, while at the same time providing many valuable jobs.

With the economic livelihoods of millions and the ecosystems of the tropics at stake,
how might we work towards affordable, timely, and scalable ways to
address the expansion and management of oil palm throughout the world?

High-resolution satellite imagery is a global, regularly-updated, and accurate source of data. Coupled with computer vision algorithms, it presents a promising opportunity for automated mapping of oil palm plantations, an important step toward understanding global impact.


# Data Description 

This year, the Global WiDS team, the West Big Data Innovation Hub, and the WiDS Datathon Committee have partnered with Planet and Figure Eight to bring more than 20,000 labeled satellite images to participants. The WiDS Datathon challenge using Kaggle’s online platform is to create a model that predicts the presence of oil palm plantations in satellite imagery. The dataset images are 3-meter spatial resolution, and each is labeled with whether an oil palm plantation appears in the image (0 for no plantation, 1 for any presence of a plantation).

The datathon task is to train a model that takes as input a satellite image and outputs a prediction of how likely it is that the image contains an oil palm plantation. Labeled training and test datasets are provided for model development; you will then upload your predictions for an unlabeled test set to Kaggle and these predictions will be used to determine the public leaderboard rankings, and the final winners of the competition.

File descriptions
train_images/image_[9-digit number].jpg - the training images from Planet
traininglabels.csv - the crowdsourced annotations/labels of presence or absence of oil palm in the training data, from Figure Eight
leaderboard_test_data/image_[9-digit number].jpg - the test images from Planet
SampleSubmission.csv - a sample submission file in the correct format
Data fields
image_id - an anonymous id unique to a given image
has_oilpalm - the annotation or label for a given image, with 0 indicating no oil palm, and 1 indicating presence of oil palm plantations
score - confidence score based on the aggregated results from crowdsourcing the annotations. This describes the level of agreement between multiple contributors, weighted by the contributor's trust score, and indicates Figure Eight's confidence in the validity of the result. For more details on how these scores are calculated, visit this article. Please note that this is extra data that need not be incorporated in your model, but may be useful. In addition, stay tuned for a blogpost focused more deeply on the data annotation process and more!

# Notebook and Methdology

Based on idea of implementing U-net architecture and Resnet50, we used data augmentation techniques of our own and pre trained library from fast.ai to implement an ANN that performed really well with accuracy of more than 99% 
