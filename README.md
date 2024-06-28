# Features

- Generate QR codes for any text or URL.
- Save QR codes in image formats.

# Installation

## 1. Python3: 
- Ensure you have Python installed. Download it from [python.org](https://www.python.org/downloads/).

### Documentation

#### Step1: Clone the repository

```bash
git clone https://github.com/BolaWagdy/QR-Code.git
cd QR-Code
```

#### Step2: Virtual Environment

```bash
python -m venv venv
source venv/bin/activate
```

#### Step3: Install Dependencies

```bash
pip install flask
pip install gunicorn
pip install -r requirements.txt
```

## 2. Docker
- For Docker-based installation, ensure Docker is installed from this steps.

```bash
# Install docker, buildx, and docker-compose
sudo apt install docker.io docker-compose docker-buildx

# Post installation steps: to run docker without sudo
sudo groupadd docker
sudo usermod -aG docker $USER
newgrp docker

# Test installation
docker run hello-world
```
### Build & Run Docker Image

```bash
docker build -t app_py .
docker run -p -p8080:8080 app_py
```

### Push to Docker Hub
> [!NOTE]  
> Username: bola278
> Reponame: app_py

#### Step 1: Tag Your Docker Image

```bash
docker tag app_py:latest bola278/app_py:latest
```

#### Step 2: Log In to Docker Hub

```bash
docker login
```

#### Step 3: Push Docker Hub

```bash
docker push bola278/app_py:latest
```

#### Step4: Pull from Docker Hub

```bash
docker pull bola278/app_py
```
