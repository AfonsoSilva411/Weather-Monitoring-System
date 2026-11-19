# MeteoAlert — Python Weather Monitoring Application

**Academic Project | 1st Year of the BSc in Computer Engineering — UTAD**

**MeteoAlert** is a Python desktop application developed to retrieve weather forecasts by city, display meteorological trends through charts, and explore basic weather alert mechanisms. It also includes a feature to send weather information by email.

The application was created as a **Group 106 academic project** during the first year of the **Bachelor's Degree in Computer Engineering** at the **University of Trás-os-Montes and Alto Douro (UTAD)**, Portugal.

## Features

- **City-based weather lookup:** Enter a city to request its weather forecast.
- **Weather forecasts:** Retrieve temperature, atmospheric pressure, humidity, and wind speed using the OpenWeatherMap API.
- **Data visualization:** Plot weather indicators using Matplotlib.
- **Change detection:** Compare weather readings and flag variations that exceed predefined thresholds.
- **Experimental hazard estimates:** Explore a logistic regression prototype that displays estimated probabilities for weather-related hazard categories.
- **Email reports:** Compose and send weather forecasts and experimental alerts using SMTP.
- **Desktop interface:** Interact with the application through Tkinter windows, buttons, and text fields.

> **Important:** The hazard probability component is a **classroom experiment, not a validated weather disaster prediction or warning system**. Its demonstration data and model must not be used for real-world risk assessment.

## Tech Stack

| Technology | Purpose |
| --- | --- |
| **Python** | Main programming language |
| **Tkinter / ttk** | Desktop graphical interface |
| **OpenWeatherMap API** | Weather forecast data source |
| **Requests** | HTTP requests |
| **Matplotlib** | Weather data charts |
| **NumPy** | Numerical data processing |
| **Scikit-learn** | Experimental logistic regression model |
| **Pillow** | Loading and displaying images |
| **smtplib** | SMTP email delivery |

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/AfonsoSilva411/API.git
cd API
```

### 2. Install dependencies

Install Python with Tkinter support (usually included in standard Python installations for Windows), then run:

```bash
python -m pip install requests pillow matplotlib numpy scikit-learn
```

### 3. Configure the application

Before running the project:

1. Obtain a valid **OpenWeatherMap API key**.
2. Configure SMTP credentials if you wish to use the email feature.
3. Make sure the image referenced in the startup screen is available in the expected directory, or update its path in the script.

### 4. Run the application

```bash
python apiMeteriologia.py
```

> This repository preserves the original academic prototype. Some changes may be needed for compatibility with current external services and Python environments.

## How It Works

1. Launch the application and open the weather lookup interface.
2. Enter the name of a city.
3. Request forecast data from OpenWeatherMap.
4. Explore forecasts and charts, view experimental alerts, or send the displayed information by email.

## Known Limitations

This project is an **educational prototype**, not production-ready software:

- The OpenWeatherMap endpoint used provides **forecast data**, not past observations. The "Historical Data" feature does not retrieve a genuine historical weather dataset.
- The hazard-estimation model uses **sample data** and is not trained or validated for reliable predictions.
- The script labels wind speed as `km/h`, but the API normally returns wind speed in `m/s`; a conversion is required for correct display.
- The Tkinter window lifecycle and general code structure could benefit from refactoring.

## Academic Context

This project provided hands-on experience with **REST API integration**, **desktop GUI development**, **data visualization**, introductory **machine learning**, and **automated email communication**.

**Degree:** BSc in Computer Engineering  
**University:** University of Trás-os-Montes and Alto Douro (UTAD)  
**Academic Year:** 1st year  
**Project Group:** 106

## Author and Credits

Developed as a group academic project, with contributions from **Afonso Silva**.

[GitHub — AfonsoSilva411](https://github.com/AfonsoSilva411)
