# oaqjp-final-project-emb-ai

## Emotion Detection Application using Watson NLP

### Project Description

This project is a web-based Emotion Detection application built as part of the IBM AI Application Development course final project. It leverages the **Watson NLP Emotion Predict** function to analyze text input and identify the dominant emotion expressed in the statement.

The application detects the following five emotions and their respective scores:
- **Anger**
- **Disgust**
- **Fear**
- **Joy**
- **Sadness**

It then identifies the **dominant emotion** — the one with the highest score — and presents the results in a clean, readable format.

---

### Project Structure

```
final_project/
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
├── templates/
│   └── index.html
├── static/
│   └── mywebscript.js
├── server.py
└── test_emotion_detection.py
```

---

### Technologies Used

- **Python 3**
- **Flask** — Web framework for deployment
- **Watson NLP Library** — Emotion Predict API (embedded, accessed via HTTP POST)
- **PyLint** — Static code analysis (10/10 score)
- **unittest** — Unit testing framework

---

### How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/ApexWolf-SuperDev/final-project-emb-ai.git
   cd final-project-emb-ai/final_project
   ```

2. Install dependencies:
   ```bash
   pip install flask requests
   ```

3. Run the Flask server:
   ```bash
   python3 server.py
   ```

4. Open your browser and navigate to:
   ```
   http://localhost:5000
   ```

---

### Running Unit Tests

```bash
cd final_project
python3 test_emotion_detection.py
```

---

### Example Output

For the input statement **"I love my life"**, the application returns:

```
For the given statement, the system response is 'anger': 0.006274985,
'disgust': 0.0025598293, 'fear': 0.009251528, 'joy': 0.9680386 and
'sadness': 0.049744144. The dominant emotion is joy.
```

---

### Error Handling

If a blank or invalid input is submitted, the application returns:

```
Invalid text! Please try again!
```

---

### Author

Developed as part of the **IBM AI Application Development with Python** course final project.