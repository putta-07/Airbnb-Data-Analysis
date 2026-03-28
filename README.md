# Airbnb Data Analysis Dashboard
## Project Overview
This project is a Power BI dashboard built to analyze Airbnb listings data. It provides insights into pricing, revenue potential, guest engagement, geographic distribution, and host performance. The dataset contains over 1 million rows of Airbnb listings with attributes such as host details, room type, price, service fee, reviews, availability, and location.

## Objectives
• Explore Airbnb market trends across neighbourhoods and room types.

• Analyze pricing structures and revenue potential.

• Understand guest behavior through reviews and booking policies.

• Visualize geographic distribution of listings.

• Evaluate host performance and identity verification.

## Dashboard Pages
The dashboard is organized into multiple pages:

### 1. Market Overview

  • Listings by neighbourhood group

  • Room availability by type

  • Instant bookability distribution

### 2. Pricing & Revenue

  • Price distribution histogram

  • Average price per room type

  • Service fee vs. price analysis

  • Revenue potential by neighbourhood

### 3. Guest Reviews & Engagement

  • Review trends over time

  • Reviews per month by room type

  • Cancellation policy impact

  • Instant bookability vs. review rate

### 4. Geographic Insights

  • Listings by neighbourhood group

  • Map of listings by latitude/longitude

  • Average price by location

  • Review density heatmap

### 5. Host Performance & Identity

  • Top hosts by number of listings

  • Host identity verification distribution

  • Average reviews per host

  • Host distribution across neighbourhoods

## Key Features
• Interactive filters: Room type, neighbourhood group, instant bookability.

• Custom DAX measures:

    DAX
    Revenue Potential = SUMX(airbnb_dataset, airbnb_dataset[price] * airbnb_dataset[availability_365])

    Average Reviews per Host =
    AVERAGEX(
    VALUES(airbnb_dataset[host id]),
    CALCULATE(AVERAGE(airbnb_dataset[number of reviews]))
    )
• Calculated columns for price ranges and host listing counts.

• Clean formatting with consistent colors, titles, and slicers.

## Dataset
The dataset includes:

• Host info: host id, host name, identity verification

• Listing info: room type, price, service fee, minimum nights, availability

• Location: neighbourhood, neighbourhood group, latitude, longitude

• Reviews: number of reviews, last review date, reviews per month

• Other attributes: cancellation policy, instant bookability, construction year

## How to Use
1. Open the .pbix file in Power BI Desktop.

2. Navigate through the pages using the bottom tabs.

3. Use slicers to filter by neighbourhood, room type, or booking options.

4. Explore insights interactively.

## Insights
• Manhattan and Brooklyn dominate Airbnb listings.

• Entire homes/apartments are the most common room type.

• Pricing varies widely, with service fees scaling alongside price.

• Guest reviews peaked around 2018 and vary by cancellation policy.

• Verified hosts and top hosts manage a significant share of listings.

## Author
Developed by PRIYANGSU DUTTA
Focus: Data visualization, simulation modeling, and dashboard design.
