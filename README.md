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
THIS SECTION NEEDS UPDATE
- Understanding Mushroom Identification
- Machine Learning Techniques
- Key Differences Between Edible and Poisonous Mushrooms
- Common Edible Mushrooms
- Essential Safety Tips
- Machine Learning Techniques

## Data Composition and Details
Our investigation aimed at identifying an appropriate dataset for the assignment led us to a CSV file derived from a study available in the University of California Irvine Machine Learning Repository. This dataset includes various features of mushrooms, facilitating the determination of their edibility status (edible or poisonous).

### Data Collection
The initial dataset we discovered was pre-cleaned and well-organized. However, it was devoid of a README file or detailed information about the variables contained within each column. This absence of documentation posed significant challenges in interpreting the variables accurately.

Despite the initial dataset being used to train our models, we sourced an alternative dataset with similar data that was well-documented. This supplementary dataset provided comprehensive details about the variables, enhancing our understanding and utilization of the data.

### Data Cleanup
During our data exploration phase, we identified that the 'Cap Shape' column contained numerous "undefined" values. Additionally, this feature was ranked low in terms of feature importance. To preserve the relevance and quality of our data, we decided to drop the 'Cap Shape' column.

Given the categorical nature of the variables in our dataset, we employed a one-hot encoding technique. This method transformed the categorical data into a series of binary columns, facilitating the effective training of our models.

## Machine Learning Techniques
In addition to traditional identification methods, we employ machine learning techniques to aid in the process. These techniques can help classify mushrooms based on their visual characteristics and other relevant features. The models used are K-Means Clustering, Logistic Regression,Random Forest, and Support Vector Machine.

### K-Means Clustering
[INSERT MODULE INFORMATION: Explanation of K-Means clustering and its application in mushroom identification, along with relevant code snippets or visualizations.]

### Logistic Regression
[INSERT MODULE INFORMATION: Explanation of Logistic Regression and its application in mushroom identification, along with relevant code snippets or visualizations.]

### Random Forest
[INSERT MODULE INFORMATION: Explanation of Random Forest and its application in mushroom identification, along with relevant code snippets or visualizations]

### Support Vector Machine (SVM)


## Study Observations
### Understanding Mushroom Features
- **Recognizing Mushroom Morphology:** Familiarize yourself with the different parts of a mushroom, such as the cap, stem, hymenium, and 
  ```python
  # Code snippet: # Get the feature importance array and list the top 20 most important features
feature_importances = rfc.feature_importances_

importances_sorted = sorted(zip(feature_importances, X.columns), reverse=True)
importances_sorted[:20]

## Habitat and Seasonal Growth
Understand the preferred habitats and seasonal growth patterns of different mushroom species. 
![Map/chart showing mushroom habitats and seasons](INSERT VISUAL: Map/chart showing mushroom habitats and seasons)

## Color and Shape
Observe the color and shape of the cap, stem, and any color changes when the mushroom is bruised. 
![Image gallery of mushroom colors and shapes](INSERT VISUAL: Image gallery of mushroom colors and shapes)

## Key Differences Between Edible and Poisonous Mushrooms

### Gill Structure and Spore Color
Edible mushrooms often have pink to brown or black gills, while poisonous varieties may have white gills and spores. 
![Comparison of gill structures and spore prints](INSERT VISUAL: Comparison of gill structures and spore prints)

### Stem Characteristics and Odors
Edible mushrooms typically have stout stems with rings or skirts, while toxic species might have a bulbous base or unpleasant odors. 
![Illustrations of stem features](INSERT VISUAL: Illustrations of stem features)

### Habitat Preferences and Groupings
Note the preferred habitats and growth patterns of mushrooms, as some poisonous varieties thrive in specific conditions. 
![Table or chart showing habitat preferences](INSERT VISUAL: Table or chart showing habitat preferences)

## Common Edible Mushrooms

### Morels
Unique conical shape, honeycomb-like cap, and hollow from cap to stem. 
![Images of morels](INSERT VISUAL: Images of morels)

### Chanterelles
Golden-yellow color, distinct fruity aroma, and forked ridges under the cap. 
![Images of chanterelles](INSERT VISUAL: Images of chanterelles)

### Oyster Mushrooms
Oyster-shaped cap, decurrent gills, and shelf-like formations on logs or trees. 
![Images of oyster mushrooms](INSERT VISUAL: Images of oyster mushrooms)

## Essential Safety Tips

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
