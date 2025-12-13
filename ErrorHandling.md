## **Error Handling**

* **Continue On Fail Enabled:**
  All social media API nodes (Facebook and X/Twitter) use *Continue On Fail* to ensure the workflow does not stop if a single post fails.

* **Failure Detection:**
  When an API call fails, the node returns error details (error message and status code), which can be used for debugging or logging.

* **Workflow Stability:**
  This approach prevents one failed post (due to rate limits, network issues, or API errors) from breaking the entire automation.

* **Future Improvements:**
  Failed posts can be logged back to Google Sheets with a status flag (e.g., `Failed`) and retry logic can be added for temporary errors such as rate limits.
