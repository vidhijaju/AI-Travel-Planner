# ✈️ AI Travel Planner

A Python Jupyter Notebook that generates a complete travel plan for any country using the Google Gemini API. Enter a country, number of days, and budget, and the notebook builds a full trip plan.

## Features

- Country overview
- 8+ famous places with descriptions, activities, best time to visit, and cost
- Place photos pulled from Wikipedia
- Interactive map of the places (Folium)
- Day-by-day itinerary (morning, afternoon, evening, food, transport, cost)
- Must-try local food
- Budget breakdown (hotel, food, transport, activities, shopping, emergency)
- Travel tips

## Tech Stack

- Python 3
- Google Gemini API (`google-genai`)
- Wikipedia API (`requests`)
- Folium
- Jupyter Notebook

## Installation

```bash
git clone https://github.com/vidhijaju/AI-Travel-Planner.git
cd <your-repo>
pip install google-genai requests folium jupyter
```

## Setup

1. Get a free API key from [Google AI Studio](https://aistudio.google.com/).
2. Save it as an environment variable. Never put the key directly in the code or commit it to GitHub.

```bash
export GEMINI_API_KEY="your-api-key"
```

3. In the notebook, load the key with:

```python
import os
API_KEY = os.environ["GEMINI_API_KEY"]
```

## Usage

1. Start Jupyter:
   ```bash
   jupyter notebook
   ```
2. Open the notebook and run all cells.
3. Enter the country, number of days, and budget when prompted.

## How It Works

1. The notebook sends a prompt to Gemini asking for a travel plan in JSON format.
2. It looks up an image for each famous place on Wikipedia.
3. It plots the places on a map and connects them with a line.
4. It prints the itinerary, food, budget, and tips.

## Limitations

- Plans are AI-generated, so check prices, opening hours, and locations before you travel.
- Some places may not have a Wikipedia image.

## Future Improvements

- Currency conversion
- Weather forecast
- Export plan to PDF
- Web app version
