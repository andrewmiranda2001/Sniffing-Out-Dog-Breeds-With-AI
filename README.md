# Title: Sniffing Out Dog Breeds With AI

# Abstract: In this project, I utilize an ensemble learning approach that combines three neural networks (VGG16, InceptionV3, and MobileNetV2) to identify dog breeds from images. My method improves breed identification accuracy and provides insights into the strengths and weaknesses of each model.



# Introduction:
The problem I am trying to solve is the identification of dog breeds from images. This is an interesting problem because accurate identification can help dog owners, breeders, and researchers better understand and manage canine populations. It can possibly be connected to CCTV cameras to help find dogs wandering the streets of specific breeds / builds. Furthermore, solving this problem contributes to the broader field of image recognition and classification.

My approach is to use an ensemble of three pre-trained neural networks (VGG16, InceptionV3, and MobileNetV2), adjust their predictions based on breed-wise test accuracy, and combine their results to improve overall identification performance.

The key components of my approach include the individual neural networks, the adjustment of their predictions using breed-wise test accuracy, and the combination of their results through a logistic regression or k-nearest neighbors model. Limitations include the reliance on pre-trained models and the need to train a classifier for each test image. It also makes it very hard to test the ensemble model as whole. 

# Setup:
I use the Stanford Dogs dataset, which contains images of 120 dog breeds. The dataset is split into training and validation sets, and I employ data augmentation to improve generalization.

The experimental setup involves running each of the three pre-trained neural networks on the input images, adjusting their predictions based on breed-wise test accuracy, and combining their results using a logistic regression or k-nearest neighbors model. I execute the experiments on a Kaggle notebook with a GPU runtime.

# Results:
Main results: My experiments show that the ensemble approach outperforms the individual neural networks in terms of breed identification accuracy. The combination of the three models provides a more robust and accurate prediction compared to relying on a single model.

Supplementary results: I experiment with different model combinations and various parameters, including the number of top predictions to consider, the threshold for the final prediction, and the choice of classifier for the final stage.

# Discussion:
The results obtained demonstrate the effectiveness of the ensemble learning approach for dog breed identification. By combining the strengths of multiple pre-trained neural networks and adjusting their predictions based on breed-wise test accuracy, I can achieve improved performance compared to using a single model. While the results are promising, it is still hard to definitevly say if the ensemble model is the better one since it is much, much slower. However, after further assessing and tweaking the models, I am planning to implement a function saving a lot of commonly used Linear Regression or KNN models to be used as part of the ensemble. This way, it will not have to re-train the simpler models if they already have been trained. 

# Conclusion:
In this project, I have developed an ensemble learning approach that combines three neural networks to accurately identify dog breeds from images. By adjusting the predictions of the individual models and combining their results, I achieve improved performance compared to using a single model. In the future, I plan to evaluate the individual models better, and then formulate a testing protocol for the ensemble machine. In future iterations of this project, I also aim to enhance the model's performance and fairness by addressing observed biases, particularly towards certain breeds like all the terriers, chihuahuas, and French bulldogs. My approach will involve refining our training data and tuning the models to mitigate overrepresentation or underrepresentation of certain breeds, ultimately striving for a more balanced and accurate breed recognition system.

This can be followed up by a Web Development project where I implement the model into an application I can deploy.  

References:
https://www.researchgate.net/publication/353693466_Dog_Breed_Classification_Using_Deep_Learning
http://cs231n.stanford.edu/reports/2015/pdfs/fcdh_FinalReport.pdf
