# 🌿 Plant Disease Detection using Deep Learning

This project implements an intelligent system for detecting plant diseases using Convolutional Neural Networks (CNN). By analyzing leaf images, the model can classify plants into 39 different categories, providing a fast and reliable way for farmers and gardeners to identify crop issues and take corrective action.

The system is built using the **PyTorch** framework and trained on the **PlantVillage dataset**.

---

## 🚀 Key Features

* **AI-Powered Diagnosis**: Uses a deep CNN to identify 39 different plant/disease combinations.
* **Modern Web Interface**: Easy-to-use Flask-based dashboard for image uploads and results.
* **Treatment Recommendations**: Provides detailed information on diseases and suggests appropriate supplements/fertilizers.
* **Supplements Marketplace**: Integrated view for exploring treatments and solutions.

---

## 💻 Tech Stack

* **AI/ML**: PyTorch, torchvision, CNN architecture
* **Backend**: Flask (Python)
* **Image Processing**: PIL, NumPy
* **Data Management**: Pandas
* **Frontend**: HTML5, CSS (Modern styling), Bootstrap 5

---

## 🛠️ Installation & Setup

### Prerequisites
* **Python 3.8+**
* A modern web browser

### Step-by-Step Setup

1. **Clone the Project**
   ```bash
   git clone <repository-url>
   cd Plant-Disease-Detection
   ```

2. **Set up Virtual Environment (Recommended)**
   ```bash
   python -m venv venv
   # Windows
   venv\Scripts\activate
   # Linux/macOS
   source venv/bin/activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Prepare the AI Model**
   * Ensure the trained model file (`plant_disease_model_1_latest.pt`) is placed inside the `Flask Deployed App` directory.
   * If using a custom model, ensure the filename matches the load path in `app.py`.

5. **Run the Application**
   ```bash
   cd "Flask Deployed App"
   python app.py
   ```

6. **Access the App**
   Navigate to `http://127.0.0.1:5000` in your web browser.

---

## 📁 Project Structure

```
Plant-Disease-Detection/
├── Flask Deployed App/      # Main application folder
│   ├── app.py               # Flask backend
│   ├── CNN.py               # Model architecture definition
│   ├── static/              # CSS, JS, and uploaded images
│   ├── templates/           # HTML templates (Home, AI Engine, About, etc.)
│   ├── disease_info.csv     # Disease metadata and descriptions
│   └── supplement_info.csv  # Supplement data and purchase links
├── Model/                   # Model training notebooks and experiments
├── test_images/             # Sample leaf images for testing the system
└── README.md                # Project documentation
```

---

## 📸 Application Preview

#### **Home Page**
A clean, welcoming interface introducing the platform's capabilities.
![Home Page](demo_images/1.png)

#### **AI Engine**
The core interface where users upload plant leaf images for analysis.
![AI Engine](demo_images/2.png)

#### **Results Page**
Detailed diagnosis including disease name, description, and prevention steps.
![Results](demo_images/3.png)

#### **Supplements & Solutions**
A curated list of products to help treat the identified diseases.
![Supplements](demo_images/4.JPG)

#### **About Section**
Insights into the mission and technology behind PlantGuard AI.
![About](demo_images/5.png)

---

## 🧪 Testing

If you don't have your own plant images, you can use the samples provided in the `test_images` folder. Each image is labeled or categorized to help you verify the model's accuracy.

