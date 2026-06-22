# Sentiment Analyzer using Django

A simple web-based Sentiment Analysis application built with **Django**, **HTML**, **CSS**, and **JavaScript**. The application analyzes user-entered text and classifies it as **Positive**, **Negative**, or **Neutral** using TextBlob.

<img width="610" height="537" alt="image" src="https://github.com/user-attachments/assets/d23d12b4-dfdd-4bb7-a147-75922854dffb" />


---

## Features

- Analyze text sentiment in real-time
- Classify text as:
  - Positive 😊
  - Negative 😞
  - Neutral 😐
- Display sentiment polarity score
- Simple and responsive UI
- Built using Django and TextBlob

---

## Tech Stack

### Frontend
- HTML5
- CSS3
- JavaScript

### Backend
- Django
- Python

### NLP Library
- TextBlob

---

## Project Structure

```text
sentiment_project/
│
├── analyzer/
│   ├── migrations/
│   ├── views.py
│   ├── urls.py
│   └── ...
│
├── sentiment_project/
│   ├── settings.py
│   ├── urls.py
│   └── ...
│
├── templates/
│   └── index.html
│
├── static/
│   ├── style.css
│   └── script.js
│
├── manage.py
├── requirements.txt
└── README.md
```

---

## Installation

### 1. Clone Repository

```bash
git clone https://github.com/yourusername/sentiment-analyzer.git
cd sentiment-analyzer
```

### 2. Create Virtual Environment

Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

Linux/Mac:

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install django
pip install textblob
```

### 4. Download TextBlob Data

```bash
python -m textblob.download_corpora
```

### 5. Run Migrations

```bash
python manage.py migrate
```

### 6. Start Development Server

```bash
python manage.py runserver
```

Open:

```text
http://127.0.0.1:8000
```

---

## How It Works

1. User enters text.
2. Django receives the text.
3. TextBlob calculates sentiment polarity.
4. Based on polarity:

```python
if polarity > 0:
    Positive
elif polarity < 0:
    Negative
else:
    Neutral
```

5. Result is displayed on the webpage.

---

## Example

### Input

```text
I absolutely love this product!
```

### Output

```text
Positive 😊
Polarity Score: 0.625
```

---

## Requirements

Create a `requirements.txt` file:

```txt
Django>=5.0
textblob>=0.18.0
```

Install using:

```bash
pip install -r requirements.txt
```

---

## Future Enhancements

- Real-time sentiment detection using AJAX
- Sentiment charts using Chart.js
- User authentication
- Sentiment history storage
- Multilingual sentiment analysis
- AI-powered sentiment analysis using Transformer models

---

## Screenshots

Add screenshots here after running the project.

```text
screenshots/
├── homepage.png
└── result.png
```

---

## Author

Your Name

GitHub: https://github.com/yourusername

---

## License

This project is licensed under the MIT License.
