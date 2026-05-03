# Environment Setup Guide

## Prerequisites
- Python 3.8+
- KNIME Analytics Platform 4.7+ (free download: https://www.knime.com/downloads)
- Power BI Desktop (free download: https://powerbi.microsoft.com/en-us/desktop/)
- Jupyter Notebook or JupyterLab

## Python Environment Setup

### 1. Clone the repository
git clone https://github.com/KubraBanu/ai-radiologists.git
cd ai-radiologists

### 2. Create a virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

### 3. Install Python dependencies
pip install -r requirements.txt

### 4. Download NLTK data
python -c "import nltk; nltk.download('punkt'); nltk.download('stopwords'); nltk.download('wordnet')"

## Dataset Access
This project uses the MIMIC-CXR dataset which requires credentialed access:
1. Complete CITI training at https://physionet.org/
2. Request access at https://physionet.org/content/mimic-cxr/
3. Once approved, download the dataset and place in a `data/` directory

## Running the Analysis
1. Open `Final_code_Radiology.ipynb` in Jupyter Notebook
2. Update the data path in Cell 1 to point to your MIMIC-CXR data directory
3. Run cells sequentially

## KNIME Workflow
1. Open KNIME Analytics Platform
2. File → Import KNIME Workflow → select `Final-Workflow-Radiology.knwf`
3. Configure data paths in the File Reader nodes
4. Execute the workflow

## Power BI Dashboard
1. Open Power BI Desktop
2. File → Open → select `Final-Dashboard-Visual-Radiology.pbix`
3. Update data source paths if prompted
