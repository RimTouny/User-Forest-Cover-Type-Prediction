# User-Forest-Cover-Type-Prediction
Predicting Colorado forest cover types using diverse ML models for classification. Baseline creation, feature selection, comparison, and tuning optimize accuracy in this University of Ottawa Master's Machine Learning course final project (2023).
       ![image](https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/4bfdb070-623f-40e9-add0-5f2739cd1565)

  - Required libraries: scikit-learn, pandas, matplotlib.
  - Execute cells in a Jupyter Notebook environment.

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
         ![Picture10](https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/0c012e10-c060-4c74-a11c-f5effb41e0ac)


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
       ![image](https://github.com/RimTouny/User-Forest-Cover-Type-Prediction/assets/48333870/98d93b8a-4eb5-4848-86df-eb6810ea18b2)


7. **First Improvement Strategy: Feature Selection:**
     - Implement feature selection methods, including filter and wrapper approaches.
     - Assess the performance of selected ML models based on the number of features versus accuracy.
     - Proceed with the best-performing feature subset and ML model for subsequent stages.
       
8. **Adding More Machine Learning Models:**
     - Implement advanced models (Random Forest, ensemble techniques) to enhance performance.
     - Compare new technique performance with the initial improvement through confusion matrices.

9. **Supervised & Unsupervised Combination via PKI:**
     - Use the best supervised model from a previous stage to determine optimal cluster numbers for improvement.
     - Implement the PKI strategy with SOFM and DNN models, aiming for better results.

10. **Applying Parameter Fine-Tuning:**
     - Experiment with different structures for the DNN PKI model to optimize performance.
     - Plot parameter tuning performance alongside the best accuracy achieved so far.

11. **Writing the Conclusion:**
     - Summarize results obtained from each improvement strategy.
     - Provide insights, experiences, and knowledge gained from the analysis in the conclusion section.


     
