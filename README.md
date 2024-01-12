# **User Forest Cover Type Prediction**
Predicting Colorado forest cover types using diverse ML models for classification. Baseline creation, feature selection, comparison ,and tuning optimize accuracy on [Forest Cover Type Prediction](https://www.kaggle.com/competitions/forest-cover-type-prediction/data) in this University of Ottawa Master's Machine Learning course final project (2023).
       ![image](https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/4bfdb070-623f-40e9-add0-5f2739cd1565)

  - Required libraries: scikit-learn, pandas, matplotlib.
  - Execute cells in a Jupyter Notebook environment.
  - The uploaded code has been executed and tested successfully within the [Google Colab](https://colab.google/) environment.

## Multi-class classification problem
Task is to classify the Forest Cover Type Prediction dataset into seven types: Spruce/Fir, Lodgepole Pine, Ponderosa Pine, Cottonwood/Willow, Aspen, Douglas-fir, and Krummholz.

### Independent Variables:
   +	54 geographical Features include 'Elevation', 'Aspect', 'Slope', 'Horizontal_Distance_To_Hydrology', 'Vertical_Distance_To_Hydrology', 'Horizontal_Distance_To_Roadways', 'Hillshade_9am', 'Hillshade_Noon', 'Hillshade_3pm', 'Horizontal_Distance_To_Fire_Points', 'Wilderness_Area1' to 'Wilderness_Area4', and 'Soil_Type1' to 'Soil_Type40'.

### Target variable:
   +	'Cover Type' column represents the target with 7 classes

## **Key Tasks Undertaken**

1. **Problem’s Overview:**
   -  Create a conceptual figure showcasing the end-to-end data flow.
   -  Illustrate insights into the problem through data flow visualization.
     

2. **Dataset’s Overview (EDA):**
   -  Present numerical information about the dataset.
      ![merge_from_ofoct (1)](https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/d3ddec7d-7d19-4b89-80e4-a7437efb9d92)


3. **General Flowchart:**
     - Develop a detailed flowchart illustrating each step of the project's implementation.
       <p align="center">
         <img src="https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/0c012e10-c060-4c74-a11c-f5effb41e0ac" />
       </p>

4. **Visualize Training and Test Sets:**
     - Generate TSNE plots separately for the training and test sets to understand the problem's complexity.
         + Problem Complexity
           ![image](https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/13796a16-0873-4ff5-a4cd-2c14832f49b4)

         + Reduction and Transformation
           ![image](https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/ff72debc-502d-43b4-ac6e-f04c24caf538)

5. **Obtain Baseline Performance:**
     - Apply diverse ML methods (KNN, LogisticRegression, SVM, DecisionTreeClassifier, Naive Bayes Classifier) to establish a baseline.
       ![merge_from_ofoct (6)](https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/d98a012b-1630-440a-8dab-01188b2ab2c5)

     - Champion Model
        ![merge_from_ofoct](https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/19dab626-e43c-4744-a773-0e403320d6ab)


7. **First Improvement Strategy: Feature Selection:**
     - Implement feature selection methods, including
        + Filter Selection Methods (Information Gain/Mutual Information , Feature Selection , Variance Threshold ,Chi-Square)
        + Wrapper Selection Methods (Forward Feature Elimination- Backward  Feature Elimination- Recursive Feature Elimination
          
     - Proceed with the best-performing feature subset and ML model for subsequent stages.
       + Champion Model in Filter Selection: Information Gain
         ```python
            Maximum of Feature Selection-K-Nearest Neighbors: 73.96721311475409
            Best number of n_components Feature Selection-K-Nearest Neighbors: 12

            Maximum of Feature Selection-Decision Tree Classifier: 76.65573770491804
            Best number of n_components Feature Selection-Decision Tree Classifier: 8
          ```       
       <p align="center">
           <img src="https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/665d2a6f-8c82-4bc2-9689-0e2e1e15a0d0"/>
       
       + Champion Model in Wrapper Selection: Recursive
         ```python
            Maximum of Recursive_FE-K-Nearest Neighbors: 73.96721311475409
            Best number of n_components Recursive_FE-K-Nearest Neighbors: 12

            Maximum of Recursive_FE-Decision Tree Classifier: 76.26229508196721
            Best number of n_components Recursive_FE-Decision Tree Classifier: 10
          ```       
       <p align="center">
           <img src="https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/943f863c-3432-4de7-aa74-abd707e9cc0c"/>
       </p>

8. **Adding More Machine Learning Models:**
     - Implement advanced models (Random Forest, ensemble techniques) to enhance performance.
       ![image](https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/f1aed811-e71b-4655-8132-750889a8b076)

     - Compare new technique performance with the initial improvement through confusion matrices.
       ![image](https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/fe32c7d5-e34c-4227-93a8-27946e1f6da7)     
