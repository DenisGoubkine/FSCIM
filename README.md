# FSCIM

This project integrates financial and supply chain data from Bloomberg, calculates vulnerability scores for a given portfolio under various scenarios, and exports the results to an Excel file for further financial analysis.

## Setup
1. Install dependencies: pip install -r requirements.txt
2. Ensure Bloomberg connectivity and appropriate entitlements.
3. Update `config.py` with the personal portfolio ID, fields, and scenario parameters (they have been removed but mock figures will reflect the intent of the project).
4. Run the application: python app.py
5. Trigger the model run: curl -X POST http://localhost:5000/run_model

## Output
The application will produce an Excel file with vulnerability scores for each security and scenario. Further financial analysis can be performed in Excel.\\

## Requirements
blpapi
Flask
numpy
pandas
xlsxwriter
