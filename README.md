For questions or collaborations, please reach out via GitHub or email.
gadbet01@gmail.com
ANAS ANWAR

# 🧠 ML Project with End-to-End MLOps Pipeline

This project demonstrates a **complete MLOps pipeline** for training, deploying, and maintaining a machine learning model using modern engineering practices. It integrates **FastAPI**, **Docker**, **MongoDB**, **CI/CD with GitHub Actions**, and **AWS S3** for a robust production-grade workflow.

---

## 🚀 Project Workflow

```mermaid
graph TD
    A[Data Ingestion] --> B[Data Validation]
    B --> C[Data Transformation]
    C --> D[Model Training]
    D --> E[Model Evaluation]
    E --> F[Model Deployment via FastAPI]
    F --> G[Model Monitoring & CI/CD (GitHub Actions)]
    G --> H[Retraining & Feedback Loop]
```

Each stage is **modular**, **version-controlled**, and **automated**, enabling smooth transitions from experimentation to production.

---

## 🛠 Tech Stack

| Category             | Tools/Services                    |
|----------------------|-----------------------------------|
| Programming Language | Python 3.10                       |
| Frameworks           | FastAPI, Scikit-learn, Pandas     |
| MLOps Tools          | Docker, GitHub Actions, DVC       |
| Cloud Services       | AWS S3                            |
| Database             | MongoDB                           |
| CI/CD                | GitHub Actions                    |
| Configuration Mgmt   | YAML, Hydra-like setup            |
| Packaging            | `setup.py`, `pyproject.toml`      |

---

## 📁 Project Structure

```
YT-MLops-Proj1-main/
├── src/                         # Core source code (training, prediction, utils)
│   ├── components/              # Pipeline steps like ingestion, transformation
│   ├── config/                  # Configuration models and schema
│   ├── pipeline/                # Training & prediction pipeline runners
│   └── logger, exception/       # Logging & exception handling
├── notebook/                    # EDA and MongoDB demos
├── config/                      # YAML config for model and schema
├── .github/workflows/aws.yaml  # CI/CD GitHub Actions pipeline
├── Dockerfile                   # Docker setup for containerization
├── requirements.txt             # Python dependencies
├── app.py                       # FastAPI entrypoint for model serving
└── README.md                    # Project documentation
```

---

## ⚙️ How to Run the Project Locally

### 🧪 1. Clone and Install

```bash
git clone https://github.com/<your-username>/YT-MLops-Proj1-main.git
cd YT-MLops-Proj1-main
pip install -r requirements.txt
```

### ⚙️ 2. Run the Pipeline

```bash
python src/pipeline/training_pipeline.py
```

### 🌐 3. Start the FastAPI App

```bash
uvicorn app:app --reload
```

Navigate to `http://localhost:8000/docs` to use the interactive API.

---

## ☁️ CI/CD with GitHub Actions

- **Trigger**: On every push to `main`
- **Build**: Docker image
- **Test**: Model & API functionality
- **Deploy**: Push to AWS S3 or EC2 (configurable)

See `.github/workflows/aws.yaml` for full CI/CD automation.

---

## 📊 MongoDB Integration

- All training metadata and logs are stored in **MongoDB** for tracking.
- Easily inspect model metrics or logs using the included notebook:
  - `notebook/mongoDB_demo.ipynb`

---

## 📌 Key Highlights

- 🔁 Full lifecycle automation
- 📦 Dockerized API with FastAPI
- 📡 Cloud storage via AWS S3
- 🧾 Model versioning & config mgmt
- 📈 Real-time scoring and CI monitoring
- ☁️ Designed for horizontal scaling

---

## 📜 License

This project is licensed under the MIT License.

---

## 📫 Contact


