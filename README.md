# 🤖 AI Data Analysis Agent

An **AI-powered Data Analysis Agent** built with **Python, Google Gemini, Pandas, KaggleHub, and Google Colab**.

This project combines traditional data analysis with Generative AI to help users understand and explore datasets using natural-language questions. The agent automatically loads a dataset, examines its structure, generates a summary, and uses **Google Gemini** to provide simple explanations and answers about the data.

## 🚀 Features

* 📊 Automatically loads and explores a dataset
* 🐼 Uses **Pandas** for data processing and analysis
* 🤖 Uses **Google Gemini AI** to analyze dataset information
* 📋 Displays dataset shape, columns, data types, and sample records
* 💡 Generates an AI-powered explanation of the dataset
* 💬 Allows users to ask questions about the dataset in natural language
* ☁️ Runs easily in **Google Colab**
* 📥 Downloads the dataset automatically using **KaggleHub**

## 🛠️ Technologies Used

* **Python**
* **Google Gemini API**
* **Pandas**
* **KaggleHub**
* **Google Colab**

## 📂 Dataset

The project uses a **Resume Dataset** downloaded through KaggleHub.

The dataset is loaded into a Pandas DataFrame and basic information such as:

* Number of rows
* Number of columns
* Column names
* Data types
* Sample records

is extracted before sending the information to Gemini for AI-powered analysis.

## ⚙️ How It Works

```text
Kaggle Dataset
      ↓
KaggleHub Download
      ↓
Load Dataset with Pandas
      ↓
Explore Dataset
      ↓
Generate Dataset Summary
      ↓
Google Gemini AI
      ↓
AI Analysis / User Questions
      ↓
Clear Natural-Language Answer
```

## 🔑 Setup

### 1. Open the Notebook

Open the project in **Google Colab**.

### 2. Install Dependencies

```python
!pip install -q google-genai pandas
```

### 3. Configure Gemini API Key

Add your Gemini API key to Google Colab Secrets with the name:

```text
GEMINI_API_KEY
```

The notebook retrieves the key securely using:

```python
GEMINI_API_KEY = userdata.get("GEMINI_API_KEY")
```

### 4. Run the Notebook

Run the cells sequentially.

The notebook will:

1. Connect to Google Gemini
2. Download the dataset using KaggleHub
3. Locate the dataset files
4. Load the CSV file using Pandas
5. Explore the dataset
6. Generate a dataset summary
7. Ask Gemini to analyze the dataset
8. Allow the user to ask questions about the data

## 💬 Example

After the dataset is loaded, you can ask questions such as:

```text
What does this dataset contain?
```

```text
What are the columns in this dataset?
```

```text
What kind of analysis can be performed on this dataset?
```

The AI agent processes the dataset information and generates a natural-language response.

## 🎯 Project Objective

The main goal of this project is to demonstrate how **Generative AI can be integrated with traditional data analysis workflows**.

Instead of manually inspecting every aspect of a dataset, users can interact with the data using simple natural-language questions.

---

⭐ If you find this project useful, consider giving the repository a star!
