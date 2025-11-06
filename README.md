# Finance Data Engineering API

A comprehensive data engineering project featuring financial data processing, ETL pipelines, and a RESTful API for accessing financial datasets.

## Features

- **ETL Pipeline**: Automated data extraction, transformation, and loading from various financial sources
- **RESTful API**: FastAPI-based endpoints for accessing financial data
- **Data Processing**: Advanced data cleaning and preprocessing
- **Database**: PostgreSQL for reliable data storage
- **Scalable Architecture**: Designed for high-volume financial data processing

## Project Structure

```
finance-data-engineering-api/
├── src/
│   ├── api/              # FastAPI application
│   ├── etl/              # ETL pipeline modules
│   ├── data/             # Data processing modules
│   ├── config/           # Configuration files
│   └── db/               # Database schemas
├── tests/                # Unit and integration tests
├── requirements.txt      # Python dependencies
├── .env.example          # Environment variables template
├── docker-compose.yml    # Docker orchestration
└── README.md            # This file
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/akhilreddy097/finance-data-engineering-api.git
cd finance-data-engineering-api
```

2. Create virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

### Start the API server:
```bash
uvicorn src.api.main:app --reload
```

### Run ETL pipeline:
```bash
python -m src.etl.pipeline
```

## API Endpoints

- `GET /api/stocks` - Get stock data
- `GET /api/currencies` - Get currency exchange rates
- `GET /api/commodities` - Get commodity prices
- `POST /api/data/process` - Submit data for processing

## Contributing

Contributions are welcome! Please feel free to submit pull requests.

## License

MIT License - See LICENSE file for details
