# Stock Price Predictor

This project utilizes LSTM (Long Short-Term Memory) neural networks to predict stock prices based on historical data. The model is implemented using TensorFlow and Keras, focusing on Apple Inc. (AAPL) stock as an example dataset.

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/SakshiFadnavis2003/Stock-Price-Predictor.git
   cd Stock-Price-Predictor
   ```

2. **Setup virtual environment (optional but recommended):**

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
   ```

3. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

## Dataset

For this example, you can use historical stock price data from sources like Yahoo Finance. Here’s how to obtain the dataset:

1. **Go to Yahoo Finance:**

   [Yahoo Finance](https://finance.yahoo.com/)

2. **Search for the stock:**

   Search for the stock symbol (e.g., Apple Inc. - AAPL).

3. **Navigate to Historical Data:**

   Click on the "Historical Data" tab.

4. **Select Time Period and Frequency:**

   Choose the desired time period and frequency (daily, weekly, monthly).

5. **Download Data:**

   Click on "Download Data" to get the historical stock prices in CSV format.

6. **Save the CSV file:**

   Save the downloaded CSV file in the `data/` directory of this project.

## Usage

1. **Prepare the dataset:**

   Download the historical stock data CSV file (e.g., `AAPL.csv`) from Yahoo Finance and place it inside the `data/` directory.

2. **Run the prediction script:**

   ```bash
   python src/stock_price_predictor.py
   ```

   This script will train the LSTM model on the data, make predictions, and display visualizations comparing actual versus predicted stock prices.

## Project Structure

- **data/:** Directory containing historical stock data CSV file (`AAPL.csv`).
- **src/:** Directory with the main script (`stock_price_predictor.py`) for model training and prediction.
- **README.md:** This file, providing project overview, installation instructions, dataset information, usage guide, and project structure.
- **requirements.txt:** List of Python packages required for the project.
- **.gitignore:** Git ignore file to exclude data files, Python caches, and virtual environments from version control.

## Results

Upon running the script, the following results are generated:

- **Stock Price Prediction Plot:** Visualizes the actual stock prices alongside predicted prices for both training and testing datasets.
- **Model Loss Plot:** Displays the training and validation loss over epochs.
- **Model MAE Plot:** Shows the Mean Absolute Error (MAE) metrics for training and validation.
- **Zoomed-In Predictions Plot:** Provides a closer look at the first 100 predictions compared to actual stock prices.

### Notes:

- **Data Source:** Ensure the `AAPL.csv` file or equivalent dataset is correctly formatted and placed in the `data/` directory before running the script.
- **Virtual Environment:** It's recommended to use a virtual environment to manage dependencies cleanly.
- **Contributions:** Contributions and feedback are welcome. Fork the repository, make improvements, and submit pull requests.

