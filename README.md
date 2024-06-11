# Mushroom Foraging: Feast or Fatal?
(Insert Visual)



## Project Team
- La Shawn Sykes
- Aaron Cranor
- Darcy DeBord
- Stephen Martinez

## Problem Summary
Ingestion of wild and potentially toxic mushrooms is a prevalent issue in the United States and many other parts of the world. Over the past 18 years, the United States has reported 133,700 cases of mushroom exposure, averaging 7,428 cases per year. These exposures are predominantly due to ingestion. Among these cases, approximately 704 exposures, or 39 per year, have resulted in major harm. Additionally, there have been 52 fatalities, averaging 2.9 per year, due to the unintentional ingestion of poisonous mushrooms by adults.<a name="section18"></a>

## Project Overview
This comprehensive study aims to equip mushroom enthusiasts with the essential knowledge and skills required for safe and effective identification of edible and poisonous mushrooms. By understanding the key differences between these two categories, foragers can confidently navigate the fascinating world of fungi while ensuring their well-being. Additionally, we leverage machine learning techniques to aid in the identification process.

## Table of Contents
## Table of Contents
1. [Understanding Mushroom Identification](#understanding-mushroom-identification)
2. [Machine Learning Techniques](#machine-learning-techniques)
3. [Key Differences Between Edible and Poisonous Mushrooms](#key-differences-between-edible-and-poisonous-mushrooms)
4. [Common Edible Mushrooms](#common-edible-mushrooms)
5. [Essential Safety Tips](#essential-safety-tips)
6. [Data Composition and Details](#data-composition-and-details)
7. [Study Observations](#study-observations)
8. [Future Recommendations](#future-recommendations)
9. [Conclusion](#conclusion)
10. [References](#references)
11. [Code Availability](#code-availability)
12. [MIT License](#mit-license)

## Data Composition and Details
Our investigation aimed at identifying an appropriate dataset for the assignment led us to a CSV file derived from a study available in the University of California Irvine Machine Learning Repository. This dataset includes various features of mushrooms, facilitating the determination of their edibility status (edible or poisonous).

### Data Collection
The initial dataset we discovered was pre-cleaned and well-organized. However, it was devoid of a README file or detailed information about the variables contained within each column. This absence of documentation posed significant challenges in interpreting the variables accurately.

Despite the initial dataset being used to train our models, we sourced an alternative dataset with similar data that was well-documented. This supplementary dataset provided comprehensive details about the variables, enhancing our understanding and utilization of the data.

### Data Cleanup
During our data exploration phase, we identified that the 'Cap Shape' column contained numerous "undefined" values. Additionally, this feature was ranked low in terms of feature importance. To preserve the relevance and quality of our data, we decided to drop the 'Cap Shape' column.

Given the categorical nature of the variables in our dataset, we employed a one-hot encoding technique. This method transformed the categorical data into a series of binary columns, facilitating the effective training of our models.

## Machine Learning Techniques
When it comes to identifying mushrooms, we can used a variety of machine learning algorithms to classify them based on their features. Here's how KMeans, Logistic Regression, Support Vector Classifier, and Random Forest were applied in mushroom identification:

KMeans
We use KMeans, an unsupervised machine learning algorithm, to cluster mushrooms into groups based on their features. For example, we cluster mushrooms into categories such as edible and poisonous based on their characteristics. By identifying patterns within the data, KMeans helps us classify mushrooms into distinct groups.

Logistic Regression
Logistic Regression, a supervised machine learning algorithm, is well-suited for binary classification tasks. In mushroom identification, we apply Logistic Regression to predict whether a mushroom is poisonous or edible based on its features. By analyzing the relationship between the input features and the binary outcome (poisonous or edible), Logistic Regression provides insights into the likelihood of a mushroom being toxic.

Support Vector Classifier (SVC)
The Support Vector Classifier is a supervised learning algorithm used for classification tasks, particularly when the data is not linearly separable. In mushroom identification, we use SVC to classify mushrooms as toxic or edible based on their features. By finding the optimal hyperplane that best separates the classes, SVC helps us make accurate predictions regarding the toxicity of mushrooms.

Random Forest
Random Forest is an ensemble learning method that leverages multiple decision trees to make predictions. In mushroom identification, we employ Random Forest to classify mushrooms as toxic or edible by considering various features and generating predictions based on the consensus of the individual trees. This ensemble approach provides robust classification results for mushroom identification.

In summary, KMeans helps us cluster mushrooms based on their characteristics, Logistic Regression and Support Vector Classifier are effective for binary classification of mushrooms, and Random Forest provides accurate classification through ensemble learning, contributing to the effective identification of mushrooms based on their attributes.

## Study Observations
### Understanding Mushroom Features
- **Recognizing Mushroom Features:** Familiarize ourselves with the different components of a mushroom, such as the odor, gill size, and population.
  
```python
# Code snippet: Get the feature importance array and list the top 20 most important features
feature_importances = rfc.feature_importances_

importances_sorted = sorted(zip(feature_importances, X.columns), reverse=True)
print(importances_sorted[:20])  # Display the top 20 most important features
```

### Seek Expert Confirmation
Always consult reputable identification guides and consider joining group forays led by experts.

### Avoid Common Mistakes and Myths
When it comes to mushrooms, there are several myths and mistakes that can have serious consequences. It's essential to understand the reality behind these misconceptions to ensure safe mushroom foraging and consumption.

Myth: All mushrooms are safe to eat if they are cooked.
Reality: Cooking does not neutralize all toxins. Some mushrooms remain poisonous even after cooking. 

Myth: Mushrooms that grow on trees are safe.
Reality: Not all tree-growing mushrooms are safe; some, like the deadly Galerina, can be fatal. 

Myth: If animals eat a mushroom, it’s safe for humans.
Reality: Animals have different tolerances and metabolisms; what’s safe for them can be deadly for humans. 

Mistake: Assuming that all mushrooms found in supermarkets are nutritious.
Reality: While many are nutritious, some may lack significant nutrients or contain harmful chemicals if not grown properly. 

Mistake: Identifying mushrooms based on pictures alone.
Reality: Accurate identification often requires detailed examination and expertise, as many mushrooms look similar. 

Myth: Poisonous mushrooms always taste bad.
Reality: Some poisonous mushrooms taste pleasant, making taste an unreliable safety test. 

Mistake: Foraging mushrooms without proper knowledge.
Reality: This can lead to accidental ingestion of toxic species, which can cause severe illness or death. 

## Future Recommendations

### Boost Accuracy with AI
Advanced artificial intelligence techniques should be explored to enhance the accuracy and reliability of our system. Implementing state-of-the-art machine learning algorithms and deep learning models could significantly improve the performance of our mushroom identification tool.

### Expand Our Dataset
To further improve the model's robustness, expanding the dataset to include a wider variety of mushrooms, particularly rare and hard-to-identify species, is essential. A more comprehensive dataset will allow the model to generalize better and perform accurately across diverse mushroom types.

### User Feedback
Incorporating user feedback and leveraging crowdsourcing can provide continuous improvement to our mushroom identification tool. Mechanisms to collect and analyze user input can help in refining the model and ensuring its practical applicability.

### Create a Mobile App
Developing an easy-to-use mobile application that utilizes our trained AI models can greatly benefit foragers in the field. Such an app would provide real-time identification of edible and poisonous mushrooms, enhancing safety and convenience for users.

## Conclusion
This study employed advanced AI techniques to enhance the performance of our classification models. By integrating various machine learning algorithms, we effectively addressed complex real-world problems. This innovative approach not only improves our current models but also paves the way for further research and advancements in AI, particularly in managing natural resources and environmental protection.

The implications of our study extend beyond enhancing the safety of mushroom foraging. It promotes sustainable practices, advances AI applications, and fosters an appreciation of the ecological significance of mushrooms. By utilizing integrated AI systems, our work demonstrates a broad and impactful contribution to technological progress and the understanding of the natural world.

## References
[1] - https://www.afdo.org/wp-content/uploads/2020/09/Basics-of-Wild-Harvested-Mushroom-Identification.pdf
[2] - https://www.mushroom-appreciation.com/mushroom-identification.html
[3] - https://mycologyst.art/identification/
[4] - https://www.wildfooduk.com/articles/how-to-tell-the-difference-between-poisonous-and-edible-mushrooms/
[5] - https://www.goodrx.com/well-being/diet-nutrition/poisonous-mushrooms-difference-between-edible
[6] - https://u.osu.edu/browncounty/2019/04/24/wild-mushrooms-edible-or-poisonous/
[7] - https://www.realmushrooms.com/mushroom-anatomy-parts/
[8] - https://grocycle.com/parts-of-a-mushroom/
[9] - https://nublumemushroom.com/blogs/blogs/the-many-parts-of-a-mushroom-a-comprehensive-guide
[10] - https://mycologyst.art/identification/where-to-find-mushrooms/
[11] - https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2268836/
[12] - https://www.naturejournalingweek.com/blogs/nature-journaling-fungi
[13] - https://mycologyst.art/identification/mushroom-morphology/
[14] - https://www.canr.msu.edu/news/identifying_mushrooms_there_is_more_to_it_than_you_might_realize
[16] - https://www.wildfooduk.com/articles/how-to-tell-the-difference-between-poisonous-and-edible-mushrooms/
[17] - https://www.quora.com/How-do-I-distinguish-wild-mushrooms-that-are-edible-to-those-that-are-toxic-to-man
[18] - https://pubmed.ncbi.nlm.nih.gov/30062915/#:~:text=Over%20the%20last%2018%20years,%25%2C%20P%20%3C%200.001

## Code Availability
The code is located within Main within the Code folder.

## MIT License
This project is licensed under the MIT License.

The MIT License is a permissive free software license that is short and to the point. It allows users considerable freedom to use, copy, modify, merge, publish, distribute, sublicense, and sell copies of the software. Here are the key points:

**Permission to Use**: Users are free to use the software for any purpose.
**Distribution**: The software can be freely distributed.
**Modification**: Users can modify the software and create derivative works.
**Attribution**: The license requires that the original authors be credited. This is typically done by including the original copyright notice in all copies or substantial portions of the software.
**No Warranty**: The software is provided "as is", without warranty of any kind, express or implied. The license explicitly states that the authors are not liable for any damages arising from the use of the software.
