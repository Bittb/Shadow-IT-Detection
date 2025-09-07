🚨 Shadow IT Detection System

An AI-powered system designed to identify and monitor unauthorized SaaS tools, devices, and services within enterprise networks. The project aims to reduce risks associated with unmanaged IT resources by offering real-time anomaly detection, risk classification, and privacy protection as the MVP.

📌 Features

🔍 Anomaly Detection – Uses NLP on logs and traffic monitoring to surface hidden or unauthorized IT assets.

🛡️ Privacy Protection MVP – Ensures sensitive user and enterprise data is prioritized in monitoring and reporting.

📊 Risk Classification – Policy-based classification of detected shadow IT tools and prioritization of high-risk incidents.

⚡ Scalable Backend – Built with Python (FastAPI/Flask) and PostgreSQL for structured storage and efficient queries.

☁️ Cloud-Native Deployment – Containerized with Docker & Kubernetes and deployable on AWS/GCP.

🔔 Automated Alerting – Sends alerts for unauthorized usage, helping reduce compliance risks.

🏗️ Tech Stack

Programming: Python

Frameworks: FastAPI / Flask

Database: PostgreSQL

ML/NLP: Scikit-learn, NLTK, spaCy

Deployment: Docker, Kubernetes, AWS/GCP

Logging/Monitoring: ELK Stack (Elasticsearch, Logstash, Kibana) [planned]

⚙️ Installation
# Clone the repository
git clone https://github.com/Bittb/Shadow-IT-Detection.git
cd Shadow-IT-Detection

# Create virtual environment
python3 -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Setup environment variables
cp .env.example .env

🚀 Usage
# Run backend API
uvicorn app.main:app --reload

# API will be available at:
http://127.0.0.1:8000


Endpoints (examples):

POST /detect → Submit logs/traffic data for shadow IT detection.

GET /assets → Retrieve all detected unauthorized assets.

GET /alerts → Fetch prioritized alerts based on policy rules.


🛡️ Security & Privacy

MVP focuses on privacy protection by ensuring no sensitive personal data is stored in raw form.

All logs are anonymized and encrypted before processing.

Compliance-ready design (GDPR, ISO 27001 alignment).

🤝 Contributing

Contributions are welcome! Please open an issue or submit a pull request with detailed explanations.

📄 License

This project is licensed under the MIT License – see the LICENSE
 file for details.
