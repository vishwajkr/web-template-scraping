# web-template-scraping

Website Scraper

This Python script scrapes an entire website, including its pages and assets (CSS, JavaScript, images, fonts), and saves them locally in a structured folder format. It uses the requests library for making HTTP requests and BeautifulSoup for parsing HTML.

Features

Downloads the main HTML files of the website.

Saves static assets such as CSS, JavaScript, images, and fonts.

Maintains folder structure for better organization.

Recursively scrapes internal links within the same domain.

Requirements

Python 3.x

Required Python libraries:

requests

beautifulsoup4

Installation

Clone or download this repository.

Install the required libraries using pip:

pip install requests beautifulsoup4

Usage

Run the script:

python scraper.py

Enter the URL of the website you want to scrape when prompted.

The scraped content will be saved in a folder named after the domain of the website (e.g., example_com).

File Structure

The downloaded files will be organized as follows:

<output_folder>/
    index.html (or other main HTML files)
    static/
        css/
        js/
        images/
        fonts/

How It Works

Main Functionality: The script starts by scraping the base URL and saving its HTML file.

Assets Downloading: It scans for static assets like CSS, JS, images, and fonts in the HTML and downloads them into their respective folders.

Internal Links: It identifies internal links (within the same domain) and recursively scrapes them.

Notes

Ensure you have the necessary permissions to scrape a website before using this tool.

The script respects the website’s internal links and does not scrape external domains.

Large websites may take significant time to scrape.

License

This project is open-source and free to use under the MIT License.

