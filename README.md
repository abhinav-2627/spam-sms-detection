# 📩 Spam SMS & Email Detector

A machine learning web application that detects whether a message is **Spam** or **Not Spam**.  
This project is built using **Flask**, **MySQL (XAMPP)**, **scikit-learn**, and a **Naïve Bayes classifier** with **TF-IDF vectorization**.  

All predictions are also stored in a **MySQL database (spamdb)**.

##  Features
- Detects SMS/Email as **Spam** or **Not Spam**
- Messages and predictions are saved in **MySQL database**
- Clean UI with **Dark Mode** & **Enter key support**
- Model trained on the `spam.csv` dataset

##  Tech Stack
- **Frontend**: HTML, CSS, JavaScript  
- **Backend**: Flask (Python)  
- **Database**: MySQL (via XAMPP)  
- **ML Model**: Multinomial Naïve Bayes + TF-IDF  

## ⚙️ Installation & Setup

### 1. Clone this repository
```bash
git clone https://github.com/your-username/spam-detector.git
cd spam-detector

3. Setup MySQL Database (via XAMPP)

Start XAMPP → Start Apache & MySQL.

Open http://localhost/phpmyadmin
CREATE DATABASE spamdb;

Inside spamdb, create a table:

CREATE TABLE messages (
    id INT AUTO_INCREMENT PRIMARY KEY,
    message TEXT NOT NULL,
    prediction VARCHAR(20) NOT NULL
);

4. Train the Model

Run the training script to generate spam_model.pkl and vectorizer.pkl:

python train.py

5. Run the Flask App
python app.py

Dataset

Dataset used: spam.csv

Labels: ham (not spam) = 0, spam = 1

Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you’d like to change.
