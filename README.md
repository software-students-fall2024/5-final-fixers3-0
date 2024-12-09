[![Machine Learning Client CI/CD Pipeline](https://github.com/software-students-fall2024/5-final-fixers3-0/actions/workflows/machine-learning-client.yml/badge.svg)](https://github.com/software-students-fall2024/5-final-fixers3-0/actions/workflows/machine-learning-client.yml)
[![Web App CI/CD Pipeline](https://github.com/software-students-fall2024/5-final-fixers3-0/actions/workflows/web-app.yml/badge.svg)](https://github.com/software-students-fall2024/5-final-fixers3-0/actions/workflows/web-app.yml)

# Journal App with Emotion Analysis

The Journal App is a web application designed to help users track their daily emotions and journal entries. The system integrates a machine-learning emotion classifier to analyze journal content and provide insights into the user's emotional state. 

---

## **Subsystems**

### **1. Machine Learning Client**
- **Functionality**: Uses a Hugging Face pre-trained model ([distilbert-base-uncased-emotion](https://huggingface.co/bhadresh-savani/distilbert-base-uncased-emotion)) to classify emotions from text.
- **Docker Image**: [ML Client on DockerHub]((https://hub.docker.com/repository/docker/dm5198/machine-learning-client/general))

### **2. Web Application**
- **Functionality**: Provides the frontend and backend for journal management.
- **Docker Image**: [Web App on DockerHub]((https://hub.docker.com/repository/docker/dm5198/web-app/general))

---

## **Team**
- [Nick Burwell](https://github.com/nickburwell)
- [Finn Eskeland](https://github.com/finn1003)
- [Jessie Kim](https://github.com/jessiekim0)
- [Dasha Miroshnichenko](https://github.com/dm5198)

---

## **Setup Instructions**

### **Prerequisites**
- Docker and Docker Compose installed
- Python 3.11+
- MongoDB
- Git
- Pipenv

---

### **Opening app**
**1. Ensure Connection to Mongo**

Download the MongoDB for VSC extension and add the database url: 'mongodb+srv://nsb8225:thefixers3.1@cluster0.8b6tk.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0' when prompted to connect to the database.

**2. Create a new virtual environment following the commands:**

```
python3 -m venv .venv

```

**Mac** 
```
source .venv/bin/activate
```

**Windows**
```
.venv\Scripts\activate
```

**3. Install Dependencies if not already installed**

```
pip install -r requirements.txt

```

Or alternatively 

```
pip install pipenv

pipenv install

pipenv shell

```

**4. Docker Compose**

Make sure that the Docker Desktop is downloaded and you are logged into your account before running the following comand:

```
docker-compose up --build

```

**5. Open the local host link for web-app and enjoy!**
