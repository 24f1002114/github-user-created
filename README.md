## Overview

This web application allows users to fetch the GitHub account creation date and age in years for a given username.  It utilizes the GitHub API to retrieve user information and displays the creation date in YYYY-MM-DD UTC format and the account age in whole years.  It also supports using a GitHub token for authorized access via the `?token=` query parameter.

## Setup

1.  Save the provided HTML code as `index.html`.
2.  Open `index.html` in your web browser.

## Usage

1.  Enter a GitHub username in the input field.
2.  Click the "Get Info" button.
3.  The account creation date and age in years will be displayed below the form.

Optionally, you can provide a GitHub token via the URL query parameter `token`. For example: `index.html?token=YOUR_GITHUB_TOKEN`. This is useful if you need to access private repositories or avoid rate limiting.  Replace `YOUR_GITHUB_TOKEN` with your actual GitHub Personal Access Token.

## Improvements from Previous Version (Round 2)

-   Added an `aria-live` alert element (`#github-status`) to report the status of the GitHub account lookup process. The alert informs the user when the lookup starts, succeeds, or fails, improving accessibility.
-   The application now displays the account age in whole years. This is calculated based on the difference between the current date and the account creation date. The account age is displayed alongside the creation date.