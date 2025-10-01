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
