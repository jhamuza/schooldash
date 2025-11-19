Sarawak Pandai Usage Dashboard

An interactive, geospatial dashboard designed to visualize and analyze the distribution of Pandai App users (Students and Teachers) across the state of Sarawak, Malaysia.

Live Demo (Replace with your actual GitHub Pages link)

📌 Project Overview

This dashboard provides stakeholders with a clear, data-driven view of educational engagement. It visualizes school-level data on an interactive map, allowing for the identification of high-performance hubs and areas requiring strategic support.

Key capabilities include dynamic filtering, dual visualization modes (Cluster/Heatmap), and AI-powered strategic analysis using the Google Gemini API.

✨ Key Features

🗺️ Interactive Visualization

Cluster Mode: Aggregates schools into clusters that expand upon zooming. Clicking a specific school marker reveals a detailed breakdown of Teacher vs. Student counts.

Heatmap Mode: Displays user density using a color gradient (Light Yellow → Dark Green) to instantly highlight hotspots of activity.

🔍 Smart Filtering & Search

Search: Instantly locate specific schools by name.

Filters: Drill down by City (e.g., Kuching, Miri) or School Type (e.g., SM Kebangsaan, SK).

Data Toggles: Switch the entire dashboard context between All Users, Students Only, or Teachers Only.

📊 Comprehensive Statistics

Key Metrics: Real-time counters for Total Students, Total Teachers, and Combined Active Users based on current filters.

Top Rankings: Dynamic top-10 lists for Cities and Schools based on user counts.

Detailed Data Table: A sortable, paginated table view of all filtered school data.

🤖 AI-Powered Strategic Insights

Strategic Query Tool: Integrated with Google Gemini 2.5 Flash. Users can ask natural language questions about the data (e.g., "Which districts have high student engagement but low teacher adoption?") and receive actionable, data-backed strategic advice.

📂 Data Management

CSV Upload: Users can upload updated Sarawak Students.csv and Sarawak Teachers.csv files to refresh the dashboard view instantly.

Secure Save: A password-protected feature allows administrators to "save" updated data into the dashboard's code for persistence (simulated for this client-side version).

🚀 Getting Started

Prerequisites

A modern web browser (Chrome, Edge, Firefox, Safari).

(Optional) A Google Gemini API Key to use the Strategic Query Tool. Get one for free at Google AI Studio.

Installation & Usage

Clone or Download this repository.

git clone [https://github.com/yourusername/sarawak-pandai-dashboard.git](https://github.com/yourusername/sarawak-pandai-dashboard.git)


Open the index.html file in your browser. No local server is required.

Setting Up AI Features (BYOK)

To enable the AI Strategic Query Tool, you need to provide your own API key. This ensures security as no keys are hardcoded in the public repository.

Click the "Settings & Data" button in the dashboard header.

In the "Gemini API Configuration" section, paste your API Key.

Click Save Key.

Note: The key is saved securely in your browser's Local Storage and is never sent to any server other than Google's API.

📁 Data Structure

The dashboard expects CSV files with the following headers for data updates:

Student CSV / Teacher CSV:

school_name,school_type,postcode,city,state_name,total_users


school_name: Name of the school (e.g., "SMK PUJUT")

school_type: Type of school (e.g., "SM KEBANGSAAN")

city: City name (e.g., "MIRI")

total_users: Integer count of active users

🛠️ Technology Stack

HTML5 / CSS3 / Vanilla JavaScript (ES6+)

Tailwind CSS (via CDN) for responsive styling.

Leaflet.js for interactive maps.

Leaflet.markercluster for cluster visualization.

Leaflet.heat for heatmap visualization.

Google Gemini API for LLM-based analysis.

🔒 Security Note

This project uses a client-side "Bring Your Own Key" architecture for the AI features. Do not commit your API key to any files in this repository. The password for the "Hardcode Data" feature is client-side only and intended for authorized administrative workflows.

Developed for Pandai Education Analytics.
