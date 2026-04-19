# 🌿 PlantGuard AI — Plant Disease Detection

An AI-powered web application that detects plant diseases from leaf images using a deep Convolutional Neural Network (CNN). Upload a photo of a plant leaf and get an instant diagnosis along with treatment recommendations.

---

## 🚀 Features

- 🤖 **Deep Learning Diagnosis** — CNN model trained on 39 plant disease classes
- ⚡ **Instant Results** — Real-time predictions directly in the browser
- 💊 **Treatment Suggestions** — Supplement and remedy recommendations for each disease
- 🛒 **Supplement Marketplace** — Browse and buy treatments for detected diseases
- 🌾 **Multi-Crop Support** — Covers 14+ crops including tomato, potato, corn, grape, and apple

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python, Flask |
| AI Model | PyTorch (CNN) |
| Image Processing | PIL, torchvision |
| Data | pandas, NumPy |
| Frontend | HTML, CSS, Bootstrap 5 |

---

## ⚙️ Getting Started

### 1. Clone the Repository

```bash
git clone <repository-url>
cd "Flask Deployed App"
```

### 2. Install Dependencies

Make sure Python 3.8+ is installed, then run:

```bash
pip install -r requirements.txt
```

### 3. Add the Trained Model

Place your trained model file in the project root (same folder as `app.py`):

```
Flask Deployed App/
├── app.py
├── plant_disease_model_1_latest.pt   ← place here
├── disease_info.csv
├── supplement_info.csv
└── ...
```

> ⚠️ If you rename the model file, update the filename in `app.py` accordingly:
> ```python
> model.load_state_dict(torch.load("your_model_name.pt"))
> ```

### 4. Run the App

```bash
python app.py
```

Then open your browser and navigate to: **http://127.0.0.1:5000**

---

## 📁 Project Structure

```
Flask Deployed App/
├── app.py                  # Main Flask application
├── CNN.py                  # CNN model architecture
├── disease_info.csv        # Disease names, descriptions & prevention steps
├── supplement_info.csv     # Supplement names, images & buy links
├── requirements.txt        # Python dependencies
├── Procfile                # Deployment config (Heroku)
├── static/                 # Static assets & uploaded images
└── templates/              # HTML templates
    ├── base.html           # Shared layout (navbar + footer)
    ├── home.html           # Landing page
    ├── index.html          # AI Engine (upload page)
    ├── submit.html         # Results page
    ├── market.html         # Supplements marketplace
    └── about.html          # About page
```

---

## 🌐 Deployment (Heroku)

The app includes a `Procfile` for Heroku deployment:

```
web: python app.py
```

Steps:
1. Create a Heroku app
2. Push your code via Git
3. Set any required environment variables
4. Ensure the model `.pt` file is included (use Git LFS for large files)

---

## 📦 Requirements

Install all dependencies with:

```bash
pip install -r requirements.txt
```

Key packages include:
- `flask`
- `torch`, `torchvision`
- `Pillow`
- `pandas`
- `numpy`
- `gunicorn` (for production deployment)

---

## 🔒 License

This project is provided for educational and research purposes. See `LICENSE` for details.
