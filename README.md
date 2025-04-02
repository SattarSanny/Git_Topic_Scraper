# GitHub Topic Scraper

This project scrapes [GitHub Topics](https://github.com/topics) to collect information about various programming topics and their top repositories. It saves this data into clean, structured `.csv` files for analysis or visualization.

---

## 📌 Features

- Scrapes all available GitHub topics.
- For each topic:
  - Extracts title, description, and URL.
  - Fetches top repositories with:
    - Username
    - Repository name
    - Star count (converted to integer)
    - Repository URL
- Saves each topic’s data in a separate CSV file inside a `data/` folder.

---

## 🚀 Technologies Used

- `requests` for HTTP requests  
- `BeautifulSoup` for HTML parsing  
- `pandas` for data manipulation  
- Python 3

---

## 🛠️ How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/github-topic-scraper.git
   cd github-topic-scraper
   ```

2. **Install required packages:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the scraper in a Jupyter Notebook or script:**
   - Open `GitHub_Topic_Scraping.ipynb` and run all cells
   - Or run the logic in a Python script

4. **Output:**
   - Check the `data/` directory for `.csv` files like:
     ```
     data/3D.csv
     data/Android.csv
     data/Machine Learning.csv
     ```

---

## 📂 Example Output

Each CSV contains:

| username   | repo_name   | stars   | repo_url                                   |
|------------|-------------|---------|--------------------------------------------|
| tensorflow | tensorflow  | 176000  | https://github.com/tensorflow/tensorflow  |

---

## 📎 Notes

- GitHub’s page layout may change. If scraping fails, update the class selectors in the code.
- Avoid running too frequently to respect GitHub’s servers.

---

## 📬 Contact

Created by [Abdul Sattar Sanny](https://github.com/SattarSanny) — feel free to reach out with questions or suggestions!

---

## ⭐ Contributing

Pull requests and stars are welcome! For major changes, please open an issue first to discuss.
