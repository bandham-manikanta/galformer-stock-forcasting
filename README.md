## Transformer based Stock Price Forecasting and Portfolio Recommendation System

### Project Structure

### Files

- **app.py**: Main Streamlit application file for the Stock Analysis Dashboard.
- **lstm_model_predictions_vals.py**: Contains functions to prepare input data and generate predictions using the LSTM model.
- **Data_Prep.py**: Script for data preparation, including loading data, feature engineering, and creating lag features.
- **Galformer.py**: Script for building, training, and evaluating the enhanced Transformer-based model (Galformer).
- **requirements.txt**: List of Python dependencies required for the project.

## Steps to Run the Streamlit App

1. **Create a Conda Environment**

   Open your terminal or command prompt and execute the following command to create a new Conda environment with TensorFlow 2.12:

   ```bash
   conda create --name <Env_Name> tensorflow=2.12 --y
   ```

   Replace `<Env_Name>` with your preferred environment name.

2. **Activate the Conda Environment**

   Activate the newly created environment:

   ```bash
   conda activate <Env_Name>
   ```

3. **Install Required Packages**

   Navigate to the project directory and install the required packages from `requirements.txt`:

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Streamlit App**

   Launch the Streamlit application:

   ```bash
   streamlit run app.py
   ```

5. **Access the Dashboard**

   Open your web browser and go to the URL provided by Streamlit (usually `http://localhost:8501`) to access the Stock Analysis Dashboard.

## Usage

- Select any one desired stock ticker from the sidebar.
- Configure the number of news articles to analyze per company.
- Click "Run Analysis" to fetch stock data, make predictions, and analyze sentiment.
- View the analysis results, including predictions, sentiment scores, and investment reasoning.
- Download the results as a CSV file if needed.
