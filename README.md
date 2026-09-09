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

## How It Works

1. Power Automate Desktop reads the origin airport, destination airport, and flight date from Excel.
2. A loop processes each route in the spreadsheet.
3. PAD opens the flight-status webpage and enters the origin and destination airport codes.
4. PAD calculates the number of months between the current date and the requested flight date.
5. JavaScript locates the calendar's **Next Month** control using its ARIA label and clicks it the required number of times.
6. PAD dynamically selects the requested day from the calendar.
7. The flight-status search is submitted.
8. PAD extracts the first displayed flight's flight number, departure time, arrival time, and status.
9. The results are written back to the corresponding row in Excel.
10. The process repeats for the remaining routes.
