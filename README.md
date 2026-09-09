# Delta Flight Status Automation

A Power Automate Desktop project that automates flight-status lookups and writes the results to Microsoft Excel.

## Project Overview

This project uses Microsoft Power Automate Desktop (PAD) to read flight search information from an Excel spreadsheet, interact with a public flight-status webpage, retrieve flight information, and write the results back to Excel.

The automation processes multiple airport routes and dynamically handles the flight date provided in the spreadsheet.

## Technologies Used

- Microsoft Power Automate Desktop
- Microsoft Excel
- JavaScript
- Regular Expressions (Regex)
- Web UI Automation

## Information Retrieved

For each route, the automation retrieves:

- Flight number
- Departure time
- Arrival time
- Flight status
