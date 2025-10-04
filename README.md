# Book Recommendation System

A content and collaborative-based filtering book recommendation system deployed as a web application. The application provides users with a list of the top 50 most popular books and allows them to search for a book to get personalized recommendations.

## 🔗 Live Demo

This project is deployed and hosted on Render.

| Status | Link |
| :--- | :--- |
| **Deployed App** | [Book Recommendation System](https://book-recommendation-system-wxru.onrender.com) |

-----

## 🌟 Features

  * **Top 50 Popular Books:** The home page displays the 50 most highly-rated and popular books based on a threshold of user ratings.
  * **Book Search & Recommendation:** Users can enter the name of a book to receive a list of highly similar book recommendations.
  * **Web Interface:** A simple, responsive web UI built with **Flask** and **Bootstrap**.
  * **Recommendation Model:** Utilizes a pre-calculated similarity matrix, likely based on a collaborative filtering or content-based approach, to find related books.

-----

## ⚙️ Installation and Setup

### Prerequisites

You need **Python 3.x** installed on your machine.

### 1\. Clone the Repository

```bash
git clone https://github.com/Haroon-89/Book-Recommendation-System
```

### 2\. Create and Activate Virtual Environment

It is recommended to use a virtual environment.

```bash
# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows:
.\venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

### 3\. Install Dependencies

Install all required Python packages using the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

### 4\. Run the Application Locally

Start the Flask application:

```bash
python app.py
```

The application will typically start on `http://127.0.0.1:5000/`.

-----

## 💻 Technologies and Libraries

This project is built using the following core technologies:

| Category | Technology | Purpose |
| :--- | :--- | :--- |
| **Web Framework** | `Flask` | Micro web framework for handling routes and serving templates. |
| **Data Processing** | `pandas`, `numpy` | Used for efficient data manipulation and numerical operations. |
| **Deployment** | `gunicorn` | WSGI HTTP Server for production deployment (e.g., on Render). |
| **Serialization** | `pickle` | Used to load the pre-processed book data and recommendation matrices. |
| **Front-End** | `HTML`, `Bootstrap 5` | For structuring and styling the web pages. |

-----

## 📁 Project Structure

```
Book-Recommendation-System-main/
├── app.py                      # Main Flask application with routes and recommendation logic
├── requirements.txt            # List of Python dependencies
├── .gitignore                  # Files and directories to be ignored by Git
├── books.pkl                   # Pickled DataFrame of book metadata
├── popular.pkl                 # Pickled DataFrame of the top 50 popular books
├── pt.pkl                      # Pickled Pivot Table (User-Item Matrix) for collaborative filtering
├── similarity_scores.pkl       # Pickled matrix containing cosine similarity scores
└── templates/
    ├── index.html              # HTML for the Home Page (Top 50 Books)
    └── recommend.html          # HTML for the Recommendation Search Page
```

-----
