# Ethiopian Medical Businesses Data Warehouse

## Project Overview
As a data engineer at Kara Solutions, this project involves building a data warehouse to store data on Ethiopian medical businesses scraped from the web and Telegram channels. The data warehouse is designed to be robust, scalable, and capable of handling the unique challenges associated with scraping and data collection from Telegram channels. Additionally, the project integrates object detection capabilities using YOLO (You Only Look Once) to enhance data analysis.

## Business Need
A data warehouse significantly enhances data analysis. With all data stored centrally, comprehensive analyses can be performed to find valuable insights about Ethiopian medical businesses. This centralized data helps identify trends, patterns, and correlations that are hard to detect with fragmented data, leading to better decision-making. A well-designed data warehouse also makes querying and reporting more efficient, enabling businesses to obtain actionable intelligence quickly and accurately.

## Project Structure
my_project/
├── main.py
├── database.py
├── models.py
├── schemas.py
├── crud.py
└── requirements.txt## Tasks Overview

### Task 1 - Data Scraping and Collection Pipeline
- **Telegram Scraping**: Utilized the Telegram API and wrote custom scripts using the `telethon` package to extract data from public Telegram channels relevant to Ethiopian medical businesses.
- **Image Scraping**: Collected images from specific Telegram channels for object detection.

### Task 2 - Data Cleaning and Transformation
- **Data Cleaning**: Removed duplicates, handled missing values, and standardized formats.
- **Data Storage**: Stored the cleaned data in a SQLite database.

### Task 3 - Object Detection Using YOLO
- **Environment Setup**: Installed necessary dependencies, including YOLO and its required libraries.
- **Object Detection**: Used the pre-trained YOLO model to detect objects in the collected images.
- **Data Storage**: Stored the detection results in a database table.

### Task 4 - Expose the Collected Data Using FastAPI
- **Environment Setup**: Installed FastAPI and Uvicorn.
- **API Development**: Created a FastAPI application to expose the collected data through various endpoints.

## Getting Started

### Prerequisites
- Python 3.7+
- SQLite
- Git

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Endework/Kara-Solutions.git
   cd ethiopian-medical-data-warehouse

 2. Create and activate a virtual environment:
    python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
3. Install the dependencies:
pip install -r requirements.txt
4. Set up the YOLO environment:
git clone https://github.com/ultralytics/yolov5.git
cd yolov5
pip install -r requirements.txt
cd ..
This version includes a completed structure and formatting for your GitHub README file. Let me know if you need any more adjustments!
