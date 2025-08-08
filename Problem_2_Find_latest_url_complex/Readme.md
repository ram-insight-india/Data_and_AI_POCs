Problem 2: Download the Latest CIUS Estimations File (FBI CDE)
📘 Task Objective
Create a Python notebook that:

Opens
👉 https://cde.ucr.cjis.gov/LATEST/webapp/#/pages/downloads

Scrolls to the Crime in the United States Annual Reports section.

In the first dropdown, selects the latest available year (detected dynamically).

In the second dropdown, selects the fixed option “CIUS Estimations.”

Clicks the Download button for that selection.

Captures and prints the final download URL.

Downloads the file and loads it with pandas (handle ZIP/CSV/Excel as needed).

Shows a preview of the dataframe (e.g., df.head()).

🛠️ What You Need to Submit
Make a new folder inside this directory using your name or GitHub username.

Put your notebook there, named:

solution.ipynb
Your notebook must clearly demonstrate:

How you locate the Crime in the United States Annual Reports panel.

How you pick the latest year (no hard-coding).

How you set “CIUS Estimations.”

The printed download URL.

The download step (saved to a local path).

Reading the data with pandas (including ZIP extraction if needed).

✅ Acceptance Criteria
Latest year is determined dynamically (parse the first dropdown options and choose max).

Second dropdown is always set to “CIUS Estimations.”

Script clicks the site’s Download button (not a manually pasted URL).

The resolved URL for the file is printed.

File is successfully downloaded and read into a pandas DataFrame.

Notebook runs headlessly—no manual clicks.

📁 Problem2_DownloadCIUSEstimations/
├─ README.md
├─ 📁 alice/
│  └─ solution.ipynb
└─ 📁 bob/
   └─ solution.ipynb


🔧 Implementation Hints (Optional but Helpful)
Because the page is a React app, use Playwright or Selenium to interact with dropdowns and the Download button reliably.

Use explicit waits until elements are visible/enabled.

After clicking Download, capture the URL via:

Playwright’s page.wait_for_event("download") and download.url, or

Reading the button’s underlying href once enabled.

Handle ZIP files with Python’s zipfile and then read inner CSV/Excel via pandas.

Happy coding! Let’s see your automation fetch the newest CIUS data like a pro. 🚀
