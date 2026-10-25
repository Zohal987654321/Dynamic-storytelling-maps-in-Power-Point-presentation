# Dynamic Storytelling Maps in PowerPoint

Turn a simple Excel table into an animated map video with **Excel 3D Maps**, then play it inside a **PowerPoint** slide.

Use it to introduce your company to investors, partners, new staff or clients: show how your business has grown across locations over time, using only Excel and PowerPoint.

<img width="1280" height="720" alt="map-preview" src="https://github.com/user-attachments/assets/787a6e49-334b-4f92-8059-7c8bf7323f89" />


---

## What's in this repository

| File | What it is |
|---|---|
| `Northline_Coffee_3D_Map_Sample.xlsx` | Starter Excel file: 18 coffee stores across Australia, monthly revenue from Jan 2024 to Sep 2026, with latitude and longitude |
| `Northline_Coffee_Growth_Review.pptx` | Example PowerPoint deck with the finished map video embedded on slide 2 |
| `images/` | Preview images used in this README |

> **Note:** Northline Coffee is a fictional company. All data is sample data created for learning.

### Inside the starter Excel file

| Sheet | Contents |
|---|---|
| **Read me** | Short build instructions |
| **Store_Sales** | 280 rows, formatted as an Excel table (`tblStoreSales`) |
| **Summary** | Revenue by state and year (SUMIFS), with a total check |

**Store_Sales columns:** Month, Store ID, Store Name, Suburb, City, State, Postcode, Country, Latitude, Longitude, Revenue (AUD), Customers

---

## Requirements

- **Excel for Windows** (Microsoft 365, 2024, 2021, 2019 or 2016). 3D Maps is not available in Excel for Mac or Excel for the web.
- **PowerPoint** for Windows or Mac (desktop app) to play the video
- **An internet connection**, because 3D Maps uses Bing to draw the map

---

## Step 1: Prepare your data

Your table needs three things:

| What | Example columns | Required? |
|---|---|---|
| **Location** | Latitude + Longitude, or Suburb, City, State, Postcode, Country | Yes |
| **A number** | Revenue, Customers, Units sold | Recommended |
| **A date** | Month | Needed for animation |

Tips:
- Click inside your data and press **Ctrl + T** to format it as a table.
- **Latitude and longitude give the most accurate map.** If you use names instead, add State and Country columns. Names like "Richmond" or "Newcastle" exist in more than one country.
- The date column must be a real Excel date, not text.

---

## Step 2: Open 3D Maps

1. Click any cell inside the table.
2. Go to **Data → Data Model → 3D Map**.
   In some versions it is under **Insert → 3D Map** (Tours group).
3. Choose **Open 3D Maps**, then **New Tour**.

The 3D Maps window opens with a globe and a **Layer Pane** on the right.

---

## Step 3: Set the fields

In the Layer Pane:

| Box | Field | What it does |
|---|---|---|
| **Location** | Latitude, Longitude (set each type) | Places each store on the map |
| **Height** | Revenue (Sum) | Taller bar = more revenue |
| **Category** | State | Gives each state its own colour |
| **Time** | Month (set to Month) | Animates the map over time |

Check the **mapping confidence** percentage. If it is below 100%, click it to see which rows did not match, then fix them in Excel.

### Time settings
Click the clock icon in Layer Options and choose how values behave over time:
- **Data shows for an instant:** each month appears, then disappears
- **Data accumulates over time:** values add up as time passes
- **Data stays in place until it is replaced:** each store shows its latest value (used in the example)

---

## Step 4: Make it look good

- **Chart type:** stacked column, clustered column, bubble, heat map or region
- **Themes:** change the map style
- **Map Labels:** show city names
- **Date box:** right-click the date, choose **Edit**, and pick a month and year format instead of date and time
- **Scene Options → Duration:** about 30–45 seconds works well for a presentation
- **Scenes:** add more scenes for close-ups (for example, start zoomed in on one city)

---

## Step 5: Export the video

1. Click **Create Video**.
2. Choose **Computers & Tablets 1080p**.
3. Optional: **Soundtrack Options** to add music.
4. Click **Create** and save the MP4.

Creating the video can take a few minutes.

---

## Step 6: Add the video to PowerPoint

1. In PowerPoint, go to **Insert → Video → This Device** and choose your MP4.
2. On the **Playback** tab, set **Start: Automatically** (or *When Clicked On*).
3. Optional: tick **Play Full Screen**.
4. Press **F5** to present.

The video is saved inside the .pptx file, so it plays on other computers too.

**If the video does not play:** a downloaded file may open in **Protected View**. Click **Enable Editing**, then try again.

---

## When to use 3D Maps (and when not to)

| Use 3D Maps for | Use something else for |
|---|---|
| A one-off story about places in a presentation | Comparing exact values (use a bar chart) |
| Showing growth or spread over time | Reports people filter and refresh every week (use Power BI) |
| Company introductions, pitches and onboarding | Sharing with Mac or web users who need to edit the map |

---

## Limitations

- Works only in Excel desktop on Windows
- Needs an internet connection
- The map opens in its own window and cannot be placed on a worksheet
- Data must be in an Excel table or the Data Model

---

## Author

Created by **Zohal Zahir**, [DATASANJ Analytics Consultancy](https://datasanj.com), Canberra, Australia.
Microsoft Fabric and Power BI consulting for small and mid-size businesses.
