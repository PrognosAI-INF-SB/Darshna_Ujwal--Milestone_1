# PrognosAI: AI-Driven Predictive Maintenance System

🚀 Project Overview
PrognosAI is a deep learning project dedicated to estimating the Remaining Useful Life (RUL) of industrial machinery using multivariate time-series sensor data. Prototyped using the NASA Commercial Modular Aero-Propulsion System Simulation (CMAPSS) dataset (specifically the FD001 subset), this system aims to recognize sequential degradation patterns and enable timely maintenance decisions.

The core objective is to minimize unplanned downtime, reduce maintenance costs, and optimize asset utilization.

🎯 Current Status: Milestone 1 Completion
Milestone 1: Data Ingestion & Preprocessing (Completed)
1. Load raw sensor data (train_FD001.txt)

2. Clean and remove static features
3. Calculate Remaining Useful Life (RUL) target
4. Scale features using Min-Max Scaler


📝Project Workflow Overview
The overall project is structured around five key milestones:
1. Data Ingestion & Preprocessing (Completed)

2. Sequence Generation: Transform data into rolling window sequences for LSTM.

3. Model Training: Design and train the LSTM model.

4. Model Evaluation: Evaluate performance using RMSE.

5. Visualization & Dashboard: Implement alerts and visualization.

📁 Project Structure
- PrognosAI/
   - data/
      - raw/                  # Contains original, untouched dataset files.
          - train_FD001.txt
      - processed/            # Stores cleaned and feature-engineered CSV (output of M1).
   - notebooks/                # Jupyter/Colab notebooks for development.
      - 1.0_data_prep.ipynb
- README.md                 # Project summary and installation guide.
- requirements.txt          # List of all Python dependencies.
- .gitignore                # Specifies files to ignore (e.g., large data outputs, environment files).

⚙️ Getting Started
1. Prerequisites
You need Python 3.8+ installed on your system.

2. Installation
- Clone the Repository:

- git clone [https://github.com/PrognosAI-INF-SB/Darshna_Ujwal--Milestone_1.git](https://github.com/PrognosAI-INF-SB/Darshna_Ujwal--Milestone_1.git) cd Darshna_Ujwal--Milestone_1

3. Install Dependencies:
- Install all required packages listed in requirements.txt.

- pip install -r requirements.txt


🟡Running the Milestone 1 Pipeline
To process the raw data and generate the output file:

Ensure the input file (train_FD001.txt) is in the data/raw/ folder.

🔵Run the notebook:

1. Execute all cells in notebooks/1.0_data_prep.ipynb
2. Output: data/processed/train_FD001_processed.csv
