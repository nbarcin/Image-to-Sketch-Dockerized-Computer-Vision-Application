# ✏️ Image-to-Sketch | Dockerized Computer Vision Application

A web-based image processing application that converts portrait images into pencil sketches using **Python, OpenCV, and Streamlit**.

The application is containerized with Docker, published on Docker Hub, and deployed on Render, making it accessible through a public URL.

## 🚀 Live Demo

**Try the application:**  
https://image-to-sketch-v1.onrender.com

**Docker Hub Image:**  
https://hub.docker.com/r/nbarcin/image-to-sketch

## 📌 Project Overview

This project demonstrates how to develop, containerize, publish, and deploy a Python-based computer vision application.

Users can upload portrait images in JPG, JPEG, or PNG format and transform them into pencil sketch effects using OpenCV image processing techniques.

## 🖥️ Application Features

- Upload images in JPG, JPEG, and PNG formats.
- Convert color images into grayscale.
- Apply image inversion.
- Use Gaussian Blur for image processing.
- Generate pencil sketch effects using the Dodge Blend technique.
- Display original and processed images side by side.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python 3.10 | Application development |
| OpenCV | Image processing |
| NumPy | Array and image manipulation |
| Pillow | Image handling |
| Streamlit | Web application interface |
| Docker | Application containerization |
| Docker Hub | Container image registry |
| Render | Cloud deployment |
| GitHub | Version control and portfolio |

## 🏗️ Application Architecture

```text
          User
           |
           v
     Web Browser
           |
           v
   Render Cloud Platform
           |
           v
      Docker Container
           |
           v
     Streamlit App
           |
           v
     OpenCV Processing
           |
           v
    Pencil Sketch Output
```

## 📂 Project Structure

```text
image-to-sketch/
│
├── app.py
├── requirements.txt
├── Dockerfile
├── .dockerignore
├── README.md
└── screenshots/
    └── app-screenshot.png
```

## ⚙️ Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/nbarcin/image-to-sketch.git
```

### 2. Navigate to the project directory

```bash
cd image-to-sketch
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the application

```bash
streamlit run app.py
```

Open your browser:

```text
http://localhost:8501
```

## 🐳 Run with Docker

### 1. Build the Docker image

```bash
docker build --platform linux/amd64 -t image-to-sketch:v1 .
```

### 2. Run the container

```bash
docker run -d \
  --platform linux/amd64 \
  -p 8501:8501 \
  --name sketch-app \
  image-to-sketch:v1
```

### 3. Access the application

```text
http://localhost:8501
```

### 4. Stop the container

```bash
docker stop sketch-app
```

## 📦 Pull from Docker Hub

You can also download and run the published Docker image directly without cloning the source code.

```bash
docker pull nbarcin/image-to-sketch:v1
```

Run the container:

```bash
docker run -d \
  --platform linux/amd64 \
  -p 8501:8501 \
  --name sketch-app \
  nbarcin/image-to-sketch:v1
```

Open:

```text
http://localhost:8501
```

## ☁️ Cloud Deployment

The application is deployed on **Render** using the Docker image published on Docker Hub.

Deployment workflow:

1. Develop the application using Python and OpenCV.
2. Build the Docker image.
3. Publish the image to Docker Hub.
4. Deploy the container image on Render.
5. Access the application through a public URL.

**Live Application:**  
https://image-to-sketch-v1.onrender.com

## 🎯 Learning Outcomes

Through this project, I gained hands-on experience with:

- Developing a computer vision application.
- Processing images using OpenCV.
- Building and managing Docker containers.
- Creating and configuring a Dockerfile.
- Publishing container images to Docker Hub.
- Deploying a containerized application to a cloud hosting platform.
- Making a Python web application publicly accessible.

## 🔮 Future Improvements

- Add multiple sketch styles and image filters.
- Allow users to download processed images.
- Improve image processing performance.
- Add image resizing and validation.
- Explore deployment using AWS container services.

## 👩‍💻 Author

**Nihal Barcin**

AI & Data | Cloud | Machine Learning

- GitHub: https://github.com/nbarcin
- LinkedIn: https://linkedin.com/in/nihal-barcin
- Kaggle: https://www.kaggle.com/nihalba
