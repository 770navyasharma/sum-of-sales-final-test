# Sales Report Calculator

## Summary
This project is a simple, single-page static website designed to calculate the total sales from an attached `data.csv` file. It parses the sales data, computes the grand total, and prominently displays the final sum on the page. The primary goal is to provide a quick and accessible sales report without requiring a complex backend or database.

## Setup
This is a static HTML, CSS, and JavaScript application. As such, no complex local server setup, package installation, or build process is required to run it.

## Usage
To view the Sales Report and the calculated total sales:

1.  **Via a Deployed Page (if available):**
    If this project is deployed, simply navigate to the live URL in your web browser. The report will load automatically.

2.  **Locally (No Deployment):**
    If you have cloned or downloaded the repository, simply open the `index.html` file directly in your web browser (e.g., by double-clicking it). Ensure that `data.csv` is located in the same directory as `index.html` for the script to find and process the data correctly.

The total sales sum will be displayed within a designated HTML element on the page, identifiable by its `id="total-sales"`.

## Code Explanation

### `index.html`
This file provides the structure and content of the web page. It sets the page title to "Sales Report" and includes a specific HTML element (e.g., a `div` or `span`) with the `id="total-sales"`. This element acts as a placeholder where the calculated total sales will be dynamically inserted by the JavaScript. It also links to the `style.css` for styling and `script.js` for functionality.

### `style.css`
This stylesheet is responsible for the visual presentation of the web page. It ensures a clean, readable layout and applies basic styling to enhance the user experience.

### `script.js`
This is the core logic of the application. It performs the following key functions:
1.  **Fetches Data:** It makes an asynchronous request to load the `data.csv` file.
2.  **Parses Data:** Once the CSV content is retrieved, it parses the data to extract the relevant sales figures.
3.  **Calculates Total:** It iterates through the parsed sales figures, summing them up to compute the grand total sales.
4.  **Updates Display:** Finally, it locates the HTML element with `id="total-sales"` and dynamically updates its content with the calculated sum, making the total sales visible to the user.

## License
This project is licensed under the MIT License.