# Mashina.kg Car Listings Scraper

This project is a script for automatically collecting links to car listings from the mashina.kg website.

## Description

The script allows you to gather links to car advertisements from a specified number of search pages on the mashina.kg website. All links are saved in JSON format to a `links.json` file.

## Requirements

- Python 3.10+
- Packages: requests, beautifulsoup4, tqdm

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/AzizaMoldosheva/parsing_2025.git
cd parsing_2025
```

### 2. Create and Activate Virtual Environment

```bash
# Install python3-venv package (if not already installed)
sudo apt install python3-venv

# Create virtual environment
python3 -m venv venv

# Activate virtual environment
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install requests beautifulsoup4==4.13.3 tqdm
```

## Usage

1. Make sure the virtual environment is activated:
```bash
source venv/bin/activate
```

2. Run the script:
```bash
python get_links.py
```

3. Enter the number of pages to parse when prompted.

4. After the script completes, all collected links will be saved to the `links.json` file.

## Project Structure

```
mashina-kg-parser/
├── get_links.py     # Main script for collecting links
├── links.json       # Output file with links
├── README.md        # Instructions file
└── venv/            # Virtual environment directory (not included in repository)
```

## Notes

- The script uses the mobile version of the mashina.kg website, which may affect the HTML structure
- When using the script, it's recommended to maintain reasonable intervals between requests to avoid creating excessive load on the server
- Please note that the executable file is named `get_links.py`