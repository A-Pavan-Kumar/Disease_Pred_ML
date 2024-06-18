# Disease_Pred_ML
In this project, disease prediction was achieved using a combination of data preprocessing, feature engineering, and machine learning techniques. Initially, data was loaded from an Excel file into a pandas DataFrame, where missing values were handled using forward fill. The data was then processed to extract disease names and corresponding symptoms, forming dictionaries that mapped each disease to its associated symptoms and occurrence counts.

Following data preparation, categorical labels (symptoms) were encoded numerically using sklearn's LabelEncoder and subsequently one-hot encoded to create a binary matrix representation of symptom presence per disease. This matrix was concatenated with the disease column and aggregated to combine all symptoms for each disease. This formed the basis of our feature set for training the machine learning model.

For model training, a Decision Tree classifier was chosen due to its ability to handle categorical data and interpretability. The dataset was split into training and testing sets using a 80-20 split. The Decision Tree model was trained on the training data and evaluated on the test set, achieving a classification accuracy score.

To visualize the decision-making process of the model, the trained Decision Tree was exported as a graphical representation using Graphviz. This provided insights into how symptoms contribute to disease prediction based on their hierarchy of importance within the tree structure.

Finally, disease prediction was conducted using the trained model on the entire dataset. Discrepancies between predicted and actual diseases were identified to assess the model's performance qualitatively.

Overall, this project demonstrates a pipeline for disease prediction using machine learning, encompassing data preprocessing, feature engineering through one-hot encoding, model training with a Decision Tree classifier, interpretability via visualization, and evaluation against actual data. This approach not only facilitates accurate disease prediction but also provides transparency in understanding how symptoms contribute to the prediction process.
