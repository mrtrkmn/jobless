# Jobless - Automated IT Job Search in Germany

This repository contains an automated job search script that scrapes IT and Software Engineering positions in Germany using JobSpy.

## Features

- 🔍 Searches for IT/Software Engineering jobs in Germany (prioritizing Berlin)
- 📅 Runs automatically every Monday at 9:00 AM UTC
- 📊 Generates CSV files with job listings
- 📦 Uploads results as GitHub Actions artifacts
- 💾 Commits results to the `jobs/` directory

## Job Search Coverage

The script searches for the following positions:
- Software Engineer
- Software Developer
- DevOps Engineer
- Site Reliability Engineer (SRE)
- System Engineer
- Backend Developer
- Full Stack Developer
- Python Developer
- Java Developer

### Job Boards Scraped
- Indeed
- LinkedIn
- Google Jobs

## Automated Workflow

The workflow runs weekly via GitHub Actions:
- **Schedule**: Every Monday at 9:00 AM UTC
- **Manual Trigger**: Can also be triggered manually via GitHub Actions UI
- **Output**: CSV files stored in the `jobs/` directory
- **Artifacts**: Results available as downloadable artifacts for 90 days

## Manual Usage

To run the script manually:

```bash
# Install dependencies
pip install -r requirements.txt

# Run the script
python searh_germany_jobs.py
```

The script will generate a CSV file in the `jobs/` directory with a timestamp in the filename (e.g., `jobs/germany_it_jobs_20260204_093000.csv`).

## CSV Output Format

The generated CSV files contain the following information:
- Job title
- Company name
- Location
- Job type
- Job board source
- Date posted
- Job URL
- Description
- Remote status
- Salary information (if available)
- Company details
- And more...

## Requirements

- Python 3.11+
- python-jobspy
- pandas

## License

This project is open source and available for anyone to use and modify.
