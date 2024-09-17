

# Customer Churn Prediction Model

This project is a **Customer Churn Prediction Model** built using an **Artificial Neural Network (ANN)**. The model is designed to predict whether a customer is likely to churn (leave a service) based on various attributes. The project is deployed using **Streamlit** for easy interaction.

## 🚀 Live Demo
You can interact with the model here: [Customer Churn Prediction Model](https://vishnushankar1-customer-churn-prediction.streamlit.app/)

## 🔍 Problem Statement
Customer churn is a critical challenge for businesses, especially in industries with high competition. Predicting which customers are likely to churn allows businesses to take preventative actions, improving customer retention and business growth.

## 📊 Features
The model takes the following customer attributes as input to predict churn:

- **Surname**: Customer's last name (used as an identifier, not for prediction)
- **Credit Score**: Customer’s credit score
- **Geography**: Customer's location
- **Gender**: Male or Female
- **Age**: Age of the customer
- **Tenure**: How many years the customer has been with the company
- **Balance**: Account balance of the customer
- **Number of Products**: Number of products the customer uses
- **Has Credit Card**: Whether the customer has a credit card (1 = Yes, 0 = No)
- **Is Active Member**: Whether the customer is an active member (1 = Yes, 0 = No)
- **Estimated Salary**: Customer’s estimated salary
- **Exited**: Target variable (1 = Customer churned, 0 = Customer retained)

## 🔧 Technologies Used
- **Python**: Core programming language for building the model
- **Pandas & NumPy**: For data manipulation and analysis
- **Scikit-learn**: For pre-processing and model building
- **TensorFlow / Keras**: For building the ANN model
- **Streamlit**: For deploying the model in an interactive web app

## 🧠 Model Overview
The model is an **Artificial Neural Network (ANN)** designed for binary classification. The target variable is **Exited**, which indicates whether the customer has churned or not. The model uses multiple layers to capture complex patterns in the customer data and predict churn.

### Architecture:
- **Input Layer**: Consists of 11 features (excluding Surname)
- **Hidden Layers**: 2-3 Dense layers with ReLU activation
- **Output Layer**: 1 node with sigmoid activation for binary classification

## 📈 Results
The model was trained on a dataset containing 10,000 customer records and achieved a significant performance in terms of accuracy and precision.

## 💻 Installation and Usage

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction
```

### 2. Install Dependencies
Make sure you have Python 3.8+ installed. Install the required libraries:
```bash
pip install -r requirements.txt
```

### 3. Run the Streamlit App
```bash
streamlit run app.py
```

### 4. View the App
Open your browser and go to `http://localhost:8501` to view the app.

## 🛠 File Structure

```
.
├── app.py              # Streamlit app script
├── churn_model.h5      # Pre-trained ANN model
├── data/               # Contains dataset
├── model_building.ipynb# Jupyter notebook for model training
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

## 📊 Dataset
The dataset consists of customer details from a banking service provider. Key columns include Credit Score, Geography, Age, and others listed under the "Features" section. It’s split into training and testing sets for model evaluation.

## 📚 Future Enhancements
- Adding more features like customer feedback, interaction history, etc.
- Optimizing the ANN architecture for better performance.
- Implementing other algorithms like Random Forest or Gradient Boosting for comparison.

## 🤝 Contributing
Feel free to submit issues or pull requests for any improvements or suggestions. Contributions are welcome!

## 📝 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
