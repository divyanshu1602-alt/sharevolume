# Company Shares Outstanding Dashboard

This is a single-file, responsive web application built with HTML, Tailwind CSS, and JavaScript. It fetches and displays the maximum and minimum common stock shares outstanding for a given company, based on data from the U.S. Securities and Exchange Commission (SEC).

## Features

-   **Dynamic Data Fetching**: Retrieves company shares outstanding data directly from the SEC's XBRL API.
-   **Filtering**: Filters data to show only entries with fiscal years (FY) greater than 2020 and valid numeric values.
-   **Max/Min Display**: Clearly highlights the maximum and minimum share outstanding figures found within the filtered data.
-   **Responsive Design**: Utilizes Tailwind CSS for a mobile-first, responsive user interface.
-   **Dynamic CIK Loading**: Supports loading data for different companies by specifying a CIK (Central Index Key) in the URL.

## How to Run

1.  **Save the file**: Save the `index.html` content to a file named `index.html` on your local machine.
2.  **Open in Browser**: Open the `index.html` file with your web browser.

    The application will automatically fetch and display data for Becton Dickinson (CIK `0000010795`) by default.

## Dynamic CIK Loading

To view data for a different company, append a `?CIK=` parameter to the URL in your browser's address bar. For example:

`index.html?CIK=0001018724` (for Apple Inc.)

Replace `0001018724` with the 10-digit CIK of the company you wish to view.

## Data Source

All data is sourced from the U.S. Securities and Exchange Commission (SEC) XBRL API.

**Important Note regarding SEC API Usage**: Per SEC guidance, a descriptive `User-Agent` header is used for API requests. The current `User-Agent` in `index.html` is `CompanySharesApp / contact@example.com`. Please consider replacing `contact@example.com` with your actual contact information if you intend to use this application extensively.

## Attachments

While `uid.txt` was mentioned as an attachment, this JSON output is strictly limited to `index.html`, `README.md`, and `LICENSE` as per the provided schema. In a full project setup, `uid.txt` would typically be provided as a separate file alongside these.

## Technologies Used

-   HTML5
-   Tailwind CSS (via CDN)
-   JavaScript
-   SEC XBRL API

## License

This project is licensed under the MIT License. See the `LICENSE` section for details.