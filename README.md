# Title: Sniffing Out Dog Breeds With AI

# Abstract: In this project, I utilize an ensemble learning approach that combines three neural networks (VGG16, InceptionV3, and MobileNetV2) to identify dog breeds from images. My method improves breed identification accuracy and provides insights into the strengths and weaknesses of each model.



# Introduction:
The problem I am trying to solve is the identification of dog breeds from images. This is an interesting problem because accurate identification can help dog owners, breeders, and researchers better understand and manage canine populations. Furthermore, solving this problem contributes to the broader field of image recognition and classification.

My approach is to use an ensemble of three pre-trained neural networks (VGG16, InceptionV3, and MobileNetV2), adjust their predictions based on breed-wise test accuracy, and combine their results to improve overall identification performance. This approach differs from other methods, which often rely on a single model for classification.

The key components of my approach include the individual neural networks, the adjustment of their predictions using breed-wise test accuracy, and the combination of their results through a logistic regression or k-nearest neighbors model. Limitations include the reliance on pre-trained models and the need to train a classifier for each test image.

# Setup:
I use the Stanford Dogs dataset, which contains images of 120 dog breeds. The dataset is split into training and validation sets, and I employ data augmentation to improve generalization.

The experimental setup involves running each of the three pre-trained neural networks on the input images, adjusting their predictions based on breed-wise test accuracy, and combining their results using a logistic regression or k-nearest neighbors model. I execute the experiments on a Kaggle notebook with a GPU runtime.

# Results:
Main results: My experiments show that the ensemble approach outperforms the individual neural networks in terms of breed identification accuracy. The combination of the three models provides a more robust and accurate prediction compared to relying on a single model.

Supplementary results: I experiment with different model combinations and various parameters, including the number of top predictions to consider, the threshold for the final prediction, and the choice of classifier for the final stage.

# Discussion:
The results obtained demonstrate the effectiveness of the ensemble learning approach for dog breed identification. By combining the strengths of multiple pre-trained neural networks and adjusting their predictions based on breed-wise test accuracy, I can achieve improved performance compared to using a single model. While the results are promising, there is potential for further improvement through the exploration of additional models or fine-tuning the pre-trained models.

# Conclusion:
In this project, I have developed an ensemble learning approach that combines three neural networks to accurately identify dog breeds from images. By adjusting the predictions of the individual models and combining their results, I achieve improved performance compared to using a single model.

References:
https://www.researchgate.net/publication/353693466_Dog_Breed_Classification_Using_Deep_Learning
http://cs231n.stanford.edu/reports/2015/pdfs/fcdh_FinalReport.pdf
