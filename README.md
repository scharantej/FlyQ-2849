## Flask Application Design

### HTML Files

- **index.html**: This file will serve as the homepage of the application, displaying a table of the cheapest flight prices to various destinations.

### Routes

- **index**: This route will render the `index.html` file and retrieve the latest cheapest flight prices using a web scraping or API call. The data will be formatted into a table within the HTML response.
- **refresh**: This route will be used to refresh the flight prices periodically (e.g., hourly). It will perform the same web scraping or API call as the `index` route but return the results in JSON format. This route can be triggered by a client-side script on the `index.html` page using AJAX.