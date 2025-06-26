# Deep-Learning-Model-Evaluation-on-Higgs-Boson-Dataset

Brief overview of the steps:

Data Loading and Exploration: 
The training and test datasets are loaded, and their structure, columns, and basic statistics are examined.
Data Preprocessing:
1. The 'Label' column is encoded from 's' and 'b' to 1 and 0.
2. Missing values (represented as -999.0) are replaced with NaN and then imputed using the median.
3. Features are separated from the target variable.
4. Features are normalized using StandardScaler.
5. The data is split into training, validation, and test sets.

Model Building and Training:
1.A baseline Multi-Layer Perceptron (MLP) model is defined and trained.
2.Architectural modifications are explored, including a deeper and wider MLP.
3.Different optimizers (RMSprop, AdamW, Nadam) are evaluated.
4.Various activation functions (LeakyReLU, SELU) are tested.
5.Regularization techniques (Batch Normalization, Dropout, L2, L1) are implemented and their effects observed.
6.Callbacks (ReduceLROnPlateau, ModelCheckpoint, EarlyStopping) are used during training.
7.The impact of different learning rates is investigated.
8.A Tree-Based baseline model (XGBoost) is trained for comparison.

Model Evaluation:
1. Performance metrics (Accuracy, Precision, Recall, F1 Score) are calculated and summarized for all trained models.
2. Confusion matrices are plotted for each model to visualize classification performance.
3. ROC-AUC curves are plotted to compare the discriminatory power of the models.
   
Summary and Reflection:
 The results of the experiments are summarized, highlighting the best-performing models. The notebook concludes with reflections on how model architecture, activation functions, regularization, learning rate, and optimizer affected performance and suggests potential areas for future improvement.
