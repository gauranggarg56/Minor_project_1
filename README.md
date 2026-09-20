# Minor_project_1
# 💬 Smart Chat Analyzer

A Python-based **chat analytics tool** that analyzes exported WhatsApp group conversations and turns raw chat data into meaningful statistics, activity patterns, and fun participant archetypes.

The **Smart Chat Analyzer** processes a WhatsApp `.txt` chat export and generates insights about group activity, messaging behavior, response patterns, frequently used words, and participant activity.

---

## 🚀 Features

### 📊 Group Overview

* Total number of messages
* Number of participants
* Chat duration
* Messages sent by each participant
* Percentage contribution of each participant

### 🔥 Activity Analysis

* Busiest day
* Busiest hour
* Hourly activity analysis
* Participant activity heatmap

### 📝 Text Analysis

* Most frequently used words
* Stop-word filtering
* Basic word-frequency analysis

### ⏱️ Response Time Analysis

* Average response time for participants
* Fastest replier
* Slowest replier

### 👻 Silent Streak Analysis

* Tracks days on which each participant was inactive
* Calculates the longest silent streak for each participant

### 🎭 Fun Personality Archetypes

The analyzer assigns participants fun chat-based archetypes such as:

* **THE SPAMMER**
* **THE GROUP MOM**
* **THE NIGHT OWL**
* **THE STORYTELLER**
* **THE DRAMA QUEEN**
* **THE GHOST**

These are based on measurable patterns in the chat and are intended purely for entertainment.

---

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* `datetime`
* File handling
* String processing
* Basic data analysis

---

## 📁 Project Structure

```text
Smart-Chat-Analyzer/
│
├── smart_chat_analyzer.py
├── hostel_bois.txt
├── README.md
└── requirements.txt
```

> The filenames can be changed according to your actual GitHub repository structure.

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/Smart-Chat-Analyzer.git
```

### 2. Open the project folder

```bash
cd Smart-Chat-Analyzer
```

### 3. Install the required dependency

```bash
pip install numpy
```

Or, if a `requirements.txt` file is included:

```bash
pip install -r requirements.txt
```

---

## 📱 Getting Your WhatsApp Chat Data

The project is designed around the text format produced by a WhatsApp chat export.

### On WhatsApp:

1. Open the group chat.
2. Open the chat options.
3. Select **Export Chat**.
4. Choose **Without Media**.
5. Save the exported `.txt` file.
6. Rename it to:

```text
hostel_bois.txt
```

7. Place it in the same directory as the Python program.

The expected format is similar to:

```text
19/09/26, 20:15 - Alice: Hey everyone!
19/09/26, 20:16 - Bob: What's up?
19/09/26, 20:17 - Charlie: Nothing much 😂
```

---

## ▶️ How to Run

Make sure the chat file is in the same directory as the Python program.

Then run:

```bash
python smart_chat_analyzer.py
```

The program will parse the chat and display the analysis directly in the terminal.

---

## 📈 Example Output

```text
GROUP OVERVIEW

Period: 01 September 2026 to 19 September 2026 (19 days)
Total messages: 2456
Participants: 8

MESSAGES PER PERSON

Alice        521 (21.2%)
Bob          438 (17.8%)
Charlie      391 (15.9%)
...

MOST ACTIVE

Busiest day: 12 September 2026
Busiest hour: 22:00 - 23:00

TOP WORDS

bro        ████████████████████ 120
college    ███████████████      91
tomorrow   ███████████          67
...

PERSONALITY ARCHETYPES

Alice      -> THE STORYTELLER
Bob        -> THE NIGHT OWL
Charlie    -> THE SPAMMER
...
```

---

## 🧠 How It Works

The analyzer follows several stages:

```text
WhatsApp Chat Export
        │
        ▼
   Parse Messages
        │
        ▼
Identify Participants
        │
        ├── Message Statistics
        ├── Activity Analysis
        ├── Word Frequency
        ├── Response Times
        ├── Silent Streaks
        └── Personality Archetypes
        │
        ▼
    Terminal Report
```

---

## 🔍 Analysis Methods

### Message Statistics

The program counts messages for every participant and calculates their percentage of the total conversation.

### Activity Heatmap

Messages are grouped according to the hour they were sent, allowing the program to identify when participants are most active.

### Word Frequency

The analyzer removes common stop words and counts the frequency of remaining words to identify commonly used terms.

### Response Time

When two consecutive messages are sent by different participants, the time gap is used to estimate the response time.

### Silent Streaks

The program tracks active days for each participant and identifies periods where they did not send any messages.

### Personality Archetypes

Simple rule-based scoring functions analyze messaging behavior and
