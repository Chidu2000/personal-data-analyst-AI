# Personal AI Data Analyst - Interactive Dashboard

## Installation

This project requires the following dependencies:

- Python 3.7 or later
- pandas
- streamlit
- numpy
- scipy
- matplotlib

You can install the required packages using pip:

```
pip install -r requirements.txt
```

## Usage

1. Run the Streamlit app:

```
streamlit run app.py
```

This will start the interactive dashboard in your web browser.

2. Upload a CSV, Excel, or JSON file to the app.
3. The app will automatically generate a list of suggested analyses based on the data.
4. Select a suggested prompt or write your own custom prompt.
5. Click the "Run analysis" button to execute the analysis.
6. The results will be displayed in the dashboard, and you can download the output as a CSV file.

## API

The main components of the API are:

- `load_data(file_or_path)`: Loads a data file into a pandas DataFrame.
- `suggest_prompts(df)`: Generates a list of suggested analyses based on the input DataFrame.
- `prompt_to_code(prompt, df)`: Converts known prompt templates into runnable Python code.
- `run_code(df, code)`: Executes the provided Python code in a restricted local namespace and returns the results.
- `ask_llm(prompt, model)`: Sends a prompt to a local Ollama language model and returns the generated output.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Testing

To run the tests, use the following command:

```
python -m unittest discover tests
```

This will run the test suite and report any failures.
