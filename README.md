# Web-Crawler-for-Beginner
 This is a simple web crawler script written in Python for beginners. The script allows you to crawl job posting webpages on LinkedIn, extract the responsibilities section, and print the job posting number, company name, and responsibilities.

### Prerequisites
To run this script, make sure you have the following installed:

Python 3: You can download Python from the official website: https://www.python.org/downloads/
Additionally, you need to install the following Python libraries:

requests: pip install requests
beautifulsoup4: pip install beautifulsoup4

### How to Use
Clone the repository or download the script to your local machine.

Open the script file (web_crawler.py) in a text editor or Python IDE of your choice.

Modify the job_posting_numbers list with the job posting numbers you want to crawl. You can replace the example job posting numbers with your desired ones.

Save the changes.

Open a command-line interface or terminal and navigate to the directory where the script is saved.

Run the script by executing the following command:

Copy code
python web_crawler.py
The script will start crawling the job posting webpages on LinkedIn and display the job posting number, company name, and responsibilities (if found) for each job posting.

### Notes
The script uses the requests library to send HTTP GET requests to the webpages and retrieve the HTML content.

The HTML content is then parsed using the beautifulsoup4 library to extract relevant information.

The script searches for the "Responsibilities" section in the HTML using various keywords commonly used for responsibilities sections.

If the "Responsibilities" section is found, the script extracts the responsibilities from the corresponding 'ul' tag.

The company name is extracted from the 'title' tag of the webpage.

The extracted information is then printed to the console.

In case the "Responsibilities" section is not found for a job posting, a message will be displayed indicating the absence of the section.

### Disclaimer
This script is intended for educational purposes only. Use it responsibly and respect the website's terms of service. LinkedIn's terms of service may prohibit scraping or crawling their website, so ensure you are authorized to perform these actions.
    
### License
This script is released under the MIT License. Feel free to modify and distribute it according to the terms of the license.