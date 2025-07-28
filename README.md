# Kafiil-Freelance-Projects-Scraper
A Python web scraper that extracts freelance project listings from Kafiil.com. It gathers data such as project title, price range, and the number of proposals, then saves it to a CSV file.

- Ethical Note
Before developing this scraper, I reviewed Kafiil’s Terms of Service and checked the site’s robots.txt file to ensure that scraping the project listings is allowed and compliant with their policies.

🔧 Features
Scrapes project listings from the first 5 pages of Kafiil.

Extracts:

 Project Title (cleaned from status prefix)

 Project Price

Number of Proposals

Outputs a structured CSV file: kafiil_project.csv.

🐍 Technologies Used
requests – for making HTTP requests

BeautifulSoup – for parsing HTML

pandas – for creating and saving the CSV file

re – for extracting proposal numbers with regex

- Getting Started
1. Clone the repository
bash
Copy
Edit
git clone https://github.com/TasneemSamie/Kafiil-Freelance-Projects-Scraper.git
cd Kafiil-Freelance-Projects-Scraper
2. Install dependencies
pip install -r requirements.txt
Or manually:
pip install requests beautifulsoup4 pandas
3. Run the script
python kafiil_scraper.py
4. Output
A file named kafiil_project.csv will be generated in your project directory.

📁 Output Sample
<img width="457" height="336" alt="image" src="https://github.com/user-attachments/assets/1ea311e9-9cb2-4f4a-a8f0-62ed6d86ec1a" />


📌 Notes
The script includes a time.sleep(2) delay between requests to be polite to the server.

It currently scrapes 5 pages; you can increase this by editing the range(1, 6) line.

Titles are cleaned to remove Arabic status words like مفتوح, مكتمل, etc.
