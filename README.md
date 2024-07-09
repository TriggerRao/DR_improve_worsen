## DR_improve_worsen

This project aims to detect if the state of Diabetic Retinopathy (DR) has improved or worsened by creating a multi-modal model trained on both images and numerical data.

### Approach

1. **Find the best suitable model for detecting DR** using cross-validation:
   - Evaluate DenseNet121, DenseNet201, VGGNet16, EfficientNetB4, and InceptionNetV3 models using K-Fold cross-validation on the image data alone.
   - Select the best performing model (VGGNet16 in this case) for further multi-modal training.

2. **Train the multi-modal model**:
   - Use the selected VGGNet16 model as the base for the multi-modal training.
   - Include 20 risk factors corresponding to each image as additional numerical data.
   - Train the model to predict the worsening or improving status of DR using both image and numerical data.

3. **Analyze the impact of additional data**:
   - Prove that including even one risk factor in addition to the image data improves the model's metrics.
   - Demonstrate that combining all 20 risk factors results in even better metrics compared to using only images or a single risk factor.

### Expected Outcomes

By following this approach, the project aims to:

1. Determine the most suitable model for detecting DR using cross-validation.
2. Develop a multi-modal model that leverages both image data and numerical risk factors to predict the worsening or improving status of DR.
3. Quantify the improvement in model performance by adding risk factors to the image data.
4. Identify the optimal combination of image data and risk factors for the best prediction accuracy.

### Potential Impact

The successful completion of this project can contribute to the early detection and monitoring of DR progression. By incorporating both image data and relevant risk factors, the multi-modal model can provide more accurate and personalized predictions, enabling healthcare professionals to make informed decisions and develop targeted treatment plans for patients with DR.
