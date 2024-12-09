[![Machine Learning Client CI/CD Pipeline](https://github.com/software-students-fall2024/5-final-fixers3-0/actions/workflows/machine-learning-client.yml/badge.svg)](https://github.com/software-students-fall2024/5-final-fixers3-0/actions/workflows/machine-learning-client.yml)
[![Web App CI/CD Pipeline](https://github.com/software-students-fall2024/5-final-fixers3-0/actions/workflows/web-app.yml/badge.svg)](https://github.com/software-students-fall2024/5-final-fixers3-0/actions/workflows/web-app.yml)

# Journal App with Emotion Analysis

The Journal App is a web application designed to help users track their daily emotions and journal entries. The system integrates a machine-learning emotion classifier to analyze journal content and provide insights into the user's emotional state. 

---

## **Subsystems**

### **1. Machine Learning Client**
- **Functionality**: Uses a Hugging Face pre-trained model [distilbert-base-uncased-emotion](https://huggingface.co/bhadresh-savani/distilbert-base-uncased-emotion) to classify emotions from text.
- **Docker Image**: [ML Client on DockerHub](https://hub.docker.com/repository/docker/dm5198/machine-learning-client/general)

### **2. Web Application**
- **Functionality**: Provides the frontend and backend for journal management.
- **Docker Image**: [Web App on DockerHub](https://hub.docker.com/repository/docker/dm5198/web-app/general)

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
**1. Clone the respository:**

```bash
    git clone https://github.com/software-students-fall2024/5-final-fixers3-0.git
    cd 5-final-fixers3-0
```
**2. Set up environment variables:**

```bash
MONGO_URI=
SECRET_KEY=
FLASK_PORT=5001
FLASK_DEBUG=1
```

**3. Create a new virtual environment following the commands:**

```bash
python3 -m venv .venv

```

**Mac** 
```bash
source .venv/bin/activate
```

**Windows**
```bash
.venv\Scripts\activate
```

**4. Install Dependencies if not already installed**

```bash
pip install -r requirements.txt

```

**5. Docker Compose**

Make sure that the Docker Desktop is downloaded and you are logged into your account before running the following comand:

```bash
docker-compose up --build

```

**6. Digital Ocean**