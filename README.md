# Fiverr Trend Monitor & Dashboard with n8n

A complete automation project built with **n8n**, **Docker**, **Google Sheets**, **XLSX export**, and a live **n8n-powered dashboard** to identify Fiverr-relevant service trends from public data sources.

This project collects trend signals, converts them into structured Fiverr niche opportunities, stores them in Google Sheets, exports them to Excel, and presents them in a simple dashboard for easy understanding.

---

## Project Summary

As a freelancer, one of the biggest challenges is knowing **what services are actually becoming more valuable in the market**.

This project solves that problem by automating the full process:

- collecting public signals from selected sources
- filtering noisy feed data
- mapping real content into Fiverr-related niches
- generating useful gig ideas and service suggestions
- storing the results in structured form
- showing the final output in a simple visual dashboard

The result is a practical market-research automation system that helps freelancers and agencies discover **what kinds of gigs are worth offering**.

---

## What This Project Does

This automation identifies service opportunities such as:

- AI automation setup
- lead generation
- short-form video editing
- SEO content / blog optimization
- Etsy SEO
- email marketing
- thumbnail design

For every matched trend signal, it can generate structured details like:

- niche
- source
- demand type
- audience
- buyer intent
- gig ideas
- keywords
- add-ons
- seasonal angles
- suggested gig titles
- evidence text

---

## Main Features

- automated trend collection using **n8n**
- scheduled workflow execution
- multi-source public trend monitoring
- filtering of invalid feed entries
- niche classification through JavaScript logic in n8n
- structured storage in **Google Sheets**
- export to **XLSX**
- live visual dashboard served through **n8n Webhook**
- simple audience-friendly dashboard design
- dashboard metrics and trend summaries

---

## Data Sources Used

The project monitors selected public sources that can reveal useful Fiverr demand patterns.

Examples include:

- Reddit communities
- job boards
- YouTube-related feeds

These sources help identify real demand signals instead of relying only on guesses or generic market assumptions.

---

## Tech Stack

- **n8n**
- **Docker**
- **Google Sheets**
- **Webhook-based dashboard**
- **XLSX export**
- **JavaScript in n8n Code nodes**

---

## Workflow Architecture

This project is built using **two separate n8n workflows**.

---

### 1. Main Trend Monitoring Workflow

This workflow collects, analyzes, and stores the data.

**Flow:**

`Schedule Trigger → Feed Seeds → RSS Read → Filter Valid Feed Items → Analyze Trends → Format for Sheets → Google Sheets / XLSX Export`

### What it does

- runs on a schedule
- loads the selected public feed URLs
- reads trend content
- filters invalid feed rows
- analyzes content into Fiverr niches
- formats the result into structured records
- stores results in Google Sheets
- exports results to Excel

---

### 2. Dashboard Workflow

This workflow reads the saved results and presents them visually.

**Flow:**

`Webhook → Get row(s) in sheet → Build Dashboard HTML → Respond to Webhook`

### What it does

- reads stored trend records from Google Sheets
- generates a clean HTML dashboard
- displays summary cards, charts, and tables
- makes the output understandable for non-technical users

---

## Dashboard Highlights

The dashboard was designed to be:

- simple
- professional
- readable
- useful for a lay audience

It includes:

- total signal count
- unique niche count
- high-intent opportunity count
- last updated timestamp
- top trending niches
- source distribution
- buyer intent mix
- top gig opportunities
- trend evidence

---

## Structured Output Fields

Each matched record contains structured fields such as:

- `generatedAt`
- `totalMatchedSignals`
- `source`
- `demandType`
- `title`
- `link`
- `niche`
- `audience`
- `buyerIntent`
- `gigIdeas`
- `keywords`
- `addons`
- `seasonal`
- `suggestedTitles`
- `evidenceText`

These fields make the data useful not just for viewing, but also for sorting, filtering, exporting, and dashboarding.

---

## Example Use Cases

This project can help with:

- discovering new Fiverr gig ideas
- identifying high-intent service niches
- finding keyword ideas for Fiverr gigs
- spotting buyer pain points from public data
- generating service add-on ideas
- creating seasonal offer ideas
- building a personal freelance market-research dashboard
- presenting automation and dashboard work in a portfolio

---

