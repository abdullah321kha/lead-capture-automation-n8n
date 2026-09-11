# Lead Capture Automation with n8n

A simple lead capture workflow built with **n8n** that automatically sends form submissions to **Google Sheets**.

## Overview

I built this project to learn how a website form can send information to an automation workflow and save it in a spreadsheet without manually copying the data.

The workflow takes the information from a form, sends it to an n8n webhook, organizes the data, and adds the lead to Google Sheets.

## Workflow

```text
Lead Capture Form
       ↓
    Webhook
       ↓
   Edit Fields
       ↓
 Google Sheets
```

## What It Does

When someone submits the form with:

* Full Name
* Email Address
* Phone Number

the information is sent to the **n8n production webhook** and automatically added as a new row in Google Sheets.

## Technologies Used

* n8n
* Webhooks
* Google Sheets
* HTML
* HTTP POST

## Workflow Steps

### 1. Lead Capture Form

The user enters:

* Name
* Email
* Phone Number

and submits the form.

### 2. Webhook

The form sends the submitted information to the **n8n production webhook** using a POST request.

### 3. Edit Fields

The incoming information is organized into the fields needed for Google Sheets.

### 4. Google Sheets

The processed information is automatically added as a new row in the connected Google Sheet.

## Example

A form submission like:

```text
Name: Abdullah
Email: abdullah@example.com
Phone: 0311XXXXXXX
```

is automatically saved in Google Sheets.

## What I Learned

While building this project, I practiced:

* Creating and using webhooks
* Working with POST requests
* Connecting an HTML form with n8n
* Passing data between workflow nodes
* Connecting n8n with Google Sheets
* Testing a production webhook
* Building a simple automation workflow

## Future Improvements

I plan to improve the project by adding:

* Email notifications for new leads
* Lead validation
* Duplicate lead checking
* CRM integration
* Lead status tracking
* Automatic follow-up emails

## Project Goal

The goal was to build something simple and understand how the different parts work together.

Instead of manually taking information from a form and putting it into a spreadsheet, the process now happens automatically.

**Small project. Real learning.**

## Author

**Abdullah Imran**

Software Engineer | AI & Automation Engineer
