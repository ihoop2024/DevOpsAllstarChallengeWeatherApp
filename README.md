# 30 Days DevOps Challenge - Weather Dashboard

Day 1: Building a weather data collection system using AWS S3 and OpenWeather API

# Weather Data Collection System - DevOps Day 1 Challenge

## Project Overview
This project is a Weather Data Collection System that demonstrates core DevOps principles by combining:
- External API Integration (OpenWeather API)
- Cloud Storage (AWS S3)
- Infrastructure as Code
- Version Control (Git)
- Python Development
- Error Handling
- Environment Management

## Features
- Fetches real-time weather data for multiple cities
- Displays temperature (°F), humidity, and weather conditions
- Automatically stores weather data in AWS S3
- Supports multiple cities tracking
- Timestamps all data for historical tracking

## Technical Architecture
- **Language:** Python 3.x
- **Cloud Provider:** AWS (S3)
- **External API:** OpenWeather API
- **Dependencies:** 
  - boto3 (AWS SDK)
  - python-dotenv
  - requests

```markdown
## Project Structure
weather-dashboard/
  src/
    __init__.py
    weather_dashboard.py
  tests/
  data/
  .env
  .gitignore
  requirements.txt

## Setup Instructions
1. Clone the repository:
--bash
git clone https://github.com/ihoop2024/DevOpsAllstarChallengeWeatherApp.git

3. Install dependencies:
bashCopypip install -r requirements.txt

4. Configure environment variables (.env):
CopyOPENWEATHER_API_KEY=your_api_key
AWS_BUCKET_NAME=your_bucket_name

4.Configure AWS credentials:
bashCopyaws configure

5. Run the application:
python src/weather_dashboard.py

What I Learned

By this being my first DevOps project with AWS.
I learned that debugging is crucial and error handling in distributed systems are essential.
Initially I ran into errors creating my S3 buckets.
However I did learn that those issues were caused by my user not having bucket permissions.
I updated my user permissions and ran the script again and I had so much joy to see the cities (objects) were being pulled into my S3 bucket.
I learned environment variable management for secure API keys.
Conducted best practices with python for API integration.
Learned git workflow for project development
Last but not least I learned cloud resource management.

## Resources
Fetched weather resources from the following link: https://openweathermap.org/api

## Results
Bucket weather-birdman-dashboard-22259 exists
Successfully created bucket weather-birdman-dashboard-22259

Fetching weather for Chicago...
Temperature: 23.9°F
Feels like: 13.48°F
Humidity: 57%
Conditions: broken clouds
Successfully saved data for Chicago to S3
Weather data for Chicago saved to S3!

Fetching weather for Miami...
Temperature: 65.61°F
Feels like: 65.3°F
Humidity: 73%
Conditions: scattered clouds
Successfully saved data for Miami to S3
Weather data for Miami saved to S3!

Fetching weather for Los Angeles...
Temperature: 70.88°F
Feels like: 68.65°F
Humidity: 21%
Conditions: smoke
Successfully saved data for Los Angeles to S3
Weather data for Los Angeles saved to S3!



