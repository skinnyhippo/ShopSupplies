# Shop Supplies Order Form

A simple web-based form for managing shop supply orders, allowing users to specify quantities and notes, generating an email with order details.

## Overview

This project provides a lightweight HTML form to track and order shop supplies. It fetches item data from an external JSON file, supports user input for quantities and notes, and creates an email with the order details. The form is designed for easy hosting on GitHub Pages.

## Features
- Displays a list of 10 shop supplies with quantity fields.
- Includes a mandatory "Order placed by" field for user identification.
- Generates an email with order details, including a user name, item quantities, and optional notes.
- Adds a "No quantities entered for reorder" note if no items are ordered.
- Compact, responsive design with browser-managed scrolling.
- Last updated timestamp for version tracking.

## Prerequisites
- A web browser (e.g., Chrome, Firefox).
- GitHub Pages (optional, for hosting).

## Setup Instructions

1. **Clone the Repository**:
   - Clone the repository to your local machine:
     ```bash
     git clone https://github.com/your-username/shop-supplies-form.git
     ```
   - Replace `your-username` and `shop-supplies-form` with your GitHub username and repository name.

2. **Prepare Files**:
   - Ensure `index.html` and `items.json` are in the root directory of the repository.
   - Verify `items.json` contains the item list in the following format:
     ```json
     [
         { "name": "Antibac Hand Soap", "subtext": "e.g., bottle" },
         { "name": "Bank Deposit Bags", "subtext": "e.g., pack of 100" },
         ...
     ]
     ```

3. **Local Testing**:
   - Install Python (if not already installed) to run a local server.
   - Navigate to the repository folder and start a server:
     ```bash
     python -m http.server 8000
     ```
   - Open your browser and go to `http://localhost:8000` to test the form.

4. **Hosting on GitHub Pages**:
   - Push the `index.html` and `items.json` files to your GitHub repository.
   - Go to **Settings** > **Pages** in your repository.
   - Set the source to the `main` branch and root directory, then save.
   - Access the live form at `https://your-username.github.io/shop-supplies-form/`.

## Usage
- Enter your name in the "Order placed by" field.
- Input quantities for the desired items.
- Add any additional notes in the "Other Notes" section.
- Click "Create Email" to generate an email with the order details.
- The email will open in your default email client with fields for manual recipient entry, subject, and pre-filled body.

## Customization
- **Update Items**: Edit `items.json` to modify the item list or subtext (e.g., change "e.g., bottle" to specific units like "32 oz bottle").
- **Adjust Layout**: Modify column widths (e.g., `w-72` for Item) or spacing in `index.html` using Tailwind CSS classes.
- **Change Date**: Update the "Last updated" text in `index.html` to reflect new versions.

## Contributing
Feel free to fork this repository, make improvements, and submit pull requests. Suggestions for additional features or bug fixes are welcome!

## License
This project is open-source under the MIT License (see LICENSE file for details).