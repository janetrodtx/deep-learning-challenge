# Charity Project Success Prediction

## Data Preprocessing

### Target Variable  
- The model predicts whether a charity project is successful (**1**) or not (**0**).  

### Feature Variables  
- All columns (except **EIN, NAME, and IS_SUCCESSFUL**) were used to train the model.  

### Removed Variables  
- **EIN and NAME** were excluded since they are just identifiers and don't help in predicting success.  

---

## Model Training & Evaluation  

### Neural Network Design  

- **Layers & Neurons:**  
  - The final model consists of **3 hidden layers** with **128, 64, and 32 neurons**.  
  - Initially, fewer layers were used, but adding more improved performance.  

- **Activation Functions:**  
  - **ReLU** was used in hidden layers to help the model learn patterns.  
  - **Sigmoid** was used in the output layer for binary classification.  

### Performance & Adjustments  

- **Final Accuracy:** **72%**, which is below the **75% target**.  
- **Optimizations Attempted:**  
  - Added more **neurons and layers** to capture complex data patterns.  
  - Tested different **activation functions** like **tanh**, but **ReLU** was more effective.  
  - Increased **epochs to 150**, allowing the model to learn longer.  

---

## Final Thoughts & Recommendations  

- The model **performs fairly well** but isn't reliable enough for funding decisions.  
- To improve accuracy:  
  - **Add more layers** or **increase neurons** per layer.  
  - **Try different activation functions** like **Leaky ReLU** or **ELU**.  
  - **Train longer** with **early stopping** to avoid overfitting.  

By implementing these improvements, the model may reach **or exceed 75% accuracy**, making it a more useful tool for predicting charity project success.  
