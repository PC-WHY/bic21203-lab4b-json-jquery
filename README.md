# Lab #4b: Client-Side Scripting (JSON and jQuery)

* **Course:** BIC21203 Web Development (Academic Session 2026/2027)
* **Name:** Pang Chew Yue
* **Student ID:** AI240178

## Overview
This repository contains the completed tasks for Lab #4b, demonstrating how to structure a valid JSON dataset, retrieve and parse JSON data asynchronously using the native JavaScript `fetch()` API, and perform equivalent DOM updates and event handling using jQuery 4.0.0.

## Repository Structure
```text
bic21203-lab4b-json-jquery/
├── README.md
├── books.json
├── books.html
└── jquery-dom.html
```

## Setup and Running Instructions
Because modern browsers block fetch() requests over the file:// protocol due to CORS security policies, Question 2 must be run through a local development server:

1) Clone or download this repository to your computer and open the folder in Visual Studio Code.
2) Install the Live Server extension in VS Code (by Ritwick Dey) if it is not already installed.
3) For Question 1 (books.json): Open books.json in VS Code to inspect the JSON dataset (or open it via Live Server to confirm valid parsing).
3) For Question 2 (books.html): Right-click books.html in the VS Code Explorer sidebar and select Open with Live Server (do not double-click the file directly via file://).
5) For Question 3 (jquery-dom.html): Open jquery-dom.html via Live Server or directly in a modern desktop browser, then click Click me to trigger the alert event.

## Question 1 — Create and Structure JSON Data
Created books.json containing a top-level "books" array with two book objects (The Great Gatsby and To Kill a Mockingbird), using double-quoted property names, string values for title and author, numeric values for publicationYear, and string arrays for genres.

Code:

<img width="565" height="417" alt="Screenshot 2026-11-19 133949" src="https://github.com/user-attachments/assets/3f2af585-a69c-491f-ae26-76730280e997" />

## Question 2 — Retrieve and Display JSON Data
Created books.html using fetch() with async/await to read books.json, display the first book's title, the second book's author, and the genres grouped by book title using document.createElement() and textContent, along with try...catch error handling for failed requests or invalid JSON.

Valid Data Output:

<img width="502" height="327" alt="Screenshot 2026-11-19 135653" src="https://github.com/user-attachments/assets/b529663d-7f33-4ad9-bd0e-58b45443bcec" />

Error Handling Output:

<img width="478" height="272" alt="Screenshot 2026-11-19 135810" src="https://github.com/user-attachments/assets/fec0f6d6-866a-4976-a49f-cc793a5e6319" />


## Question 3 — Compare Native JavaScript and jQuery
Created jquery-dom.html importing the official jQuery 4.0.0 full-build CDN (https://code.jquery.com/jquery-4.0.0.min.js) to update #myElement via .text(), style #myDIV via .addClass("myStyle"), and handle #myButton clicks via .on("click", ...).

Output:

<img width="951" height="207" alt="Screenshot 2026-11-19 140118" src="https://github.com/user-attachments/assets/efa08b88-8615-459f-9396-9aa8da7d013f" />
