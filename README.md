# Data Visualization Agent (ADK)

This project is an interactive Colab/Notebook application that generates Python code for data visualizations using the Google Gemini LLM, based on user requests, and applies it to a given dataset.

## Features

- Natural language to visualization: Generates Python visualization code from user prompts using the Google Generative AI (Gemini) API.
- Integrates with pandas, matplotlib, and seaborn.
- Allows you to upload and analyze your own dataset.
- Automatically saves and displays generated charts.
- Modular structure: `agent.py` (code generator), `tools.py` (code executor).

## How It Works

1. Installs required libraries and sets up the Gemini API key.
2. Receives a visualization request from the user (e.g., "draw a bar chart of the top 3 states by sales").
3. Sends a prompt to Gemini, which returns Python code.
4. Executes the code on a sample dataset and generates a chart.
5. Chart is automatically displayed in the notebook.

## Usage

1. **Open in Google Colab or run locally.**
2. Obtain a [Google Gemini API key](https://makersuite.google.com/app/apikey) and add it as `GOOGLE_API_KEY` in Colab secrets.
3. Run the notebook step by step.
4. Upload your dataset to the `uploads/` folder, or use the sample data provided.
5. Enter your visualization request in English or Turkish.

## File Structure

- `Data_Viz_Agent_ADK.ipynb` — Main notebook file.
- `agent.py` — Module for generating visualization code.
- `tools.py` — Module for executing the generated code and saving the chart.
- `uploads/state_sales.csv` — Sample dataset (you can replace this with your own).
- `outputs/visualization.png` — Generated charts are saved here.

## Requirements

All required libraries are listed in the `requirements.txt` file below.

## Contribution

To contribute, please fork the repository and open a pull request or create an issue.

## License

MIT
