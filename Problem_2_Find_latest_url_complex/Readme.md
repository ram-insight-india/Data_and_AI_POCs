# Problem 2: Download the Latest CIUS Estimations File (FBI CDE)

## 📘 Task Objective
Create a Python notebook that:

1. Opens
👉 https://cde.ucr.cjis.gov/LATEST/webapp/#/pages/downloads
2. Scrolls to the Crime in the United States Annual Reports section.
   
3. In the first dropdown, selects the latest available year (detected dynamically).

4. In the second dropdown, selects the fixed option “CIUS Estimations.”

5. Clicks the Download button for that selection.

6. Captures and prints the final download URL. 

7. Downloads the file and loads it with pandas (handle ZIP/CSV/Excel as needed).

8. Shows a preview of the dataframe (e.g., df.head()).

---

## 🛠️ What You Need to Submit
- Make a new folder inside this directory using your name or GitHub username.
- Put your notebook there, named:
solution.ipynb
- Your notebook must clearly demonstrate:
   - How you locate the Crime in the United States Annual Reports panel.
   - How you pick the latest year (no hard-coding).

   - How you set “CIUS Estimations.”
   - The printed download URL.
   - The download step (saved to a local path).
   - Reading the data with pandas (including ZIP extraction if needed).
 
---

## ✅ Acceptance Criteria
- Latest year is determined dynamically (parse the first dropdown options and choose max).

- Second dropdown is always set to “CIUS Estimations.”

- Script clicks the site’s Download button (not a manually pasted URL).

- The resolved URL for the file is printed.

- File is successfully downloaded and read into a pandas DataFrame.

- Notebook runs headlessly—no manual clicks.

---

## 📦 Example Folder Structure

📁 Problem_2_Find_latest_url_complex/
- README.md
- 📁 alice/
   - solution.ipynb
- 📁 bob/
  - solution.ipynb

---

## 🔧 Implementation Hints (Optional but Helpful)
- Because the page is a React app, use Playwright or Selenium to interact with dropdowns and the Download button reliably.

- Use explicit waits until elements are visible/enabled.

---

Happy coding! Let’s see your automation fetch the newest CIUS data like a pro. 🚀

