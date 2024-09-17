# Currency Conversion Script

This script allows users to convert a base currency to multiple other currencies using the Free Currency API. The script continuously prompts the user for a base currency and displays the conversion rates for a predefined list of currencies.

## Features

- Converts a base currency to multiple other currencies.
- Uses the Free Currency API to fetch the latest conversion rates.
- Continuously prompts the user for a base currency until they choose to quit.

## Requirements

- Python 3.x
- `requests` module (`pip install requests`)
- Free Currency API key

## Usage

1. **Clone the repository** (if applicable) or download the script file.

2. **Install the required module**:
   ```bash
   pip install requests
   ```

3. **Edit the script**:
   - Replace `'fca***` with your Free Currency API key.
   - Optionally, modify the `CURRENCIES` list to include the currencies you want to convert to.

4. **Run the script**:
   ```bash
   python script_name.py
   ```

5. **Use the script**:
   - Enter the base currency code when prompted (e.g., `USD`, `EUR`).
   - Enter `q` to quit the script.

## How It Works

1. The script defines the API key, base URL, and a list of target currencies.
2. The `convert_currency` function constructs the API request URL, fetches the conversion rates, and returns the data.
3. The script continuously prompts the user for a base currency and displays the conversion rates for the target currencies.
4. The user can quit the script by entering `q`.

## Notes

- Ensure you have a valid API key from the Free Currency API.
- The script handles invalid currency inputs by displaying an error message and prompting the user again.
