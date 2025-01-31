# week-8-python-assignment-Weather-Project

# Weather Project

This project fetches real-time weather data using a weather API and displays it. The project is built using Python and requires a `.env` file to securely store your API key.

## Requirements

- Python 3.x
- `python-dotenv` library (for loading environment variables)
- `requests` library (for making HTTP requests to the API)

## Setup

### 1. Clone the repository:
```bash
git clone https://github.com/yourusername/weather-project.git
cd weather-project
```

### 2. Create and activate the virtual environment:
For **Windows** (Command Prompt):
```bash
python -m venv myenv
myenv\Scripts\activate
```

For **Mac/Linux**:
```bash
python3 -m venv myenv
source myenv/bin/activate
```

### 3. Install the required dependencies:
```bash
pip install -r requirements.txt
```

### 4. Set up your `.env` file:
In the root directory of the project, create a `.env` file and add your API key:
```
API_KEY=your_api_key_here
```
> **Important:** The API key is confidential, so keep it secure. Do not share or commit the `.env` file to version control (e.g., GitHub). You can obtain your API key by registering with a weather API provider such as [OpenWeatherMap](https://openweathermap.org/).

### 5. Run the application:
After setting up your `.env` file and activating your virtual environment, you can run the project with:
```bash
python app.py
```

### 6. Example output:
Once the application is running, it will prompt you to enter a city name. After entering the city, it will display the weather information, for example:
```
Enter the name of the city: London
Weather in London:
Temperature: 15°C
Humidity: 60%
Pressure: 1015 hPa
Condition: Clear sky
```

## How it works:

- The script makes a request to the weather API using the `requests` library and fetches real-time weather data for a specified city.
- It loads the API key from the `.env` file using the `python-dotenv` library.
- The weather details, including temperature, humidity, pressure, and condition, are then displayed in the terminal.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

