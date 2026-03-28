# Data Visualization Video Plan

csv data: research interest data sets related to AI

Use the Remotion best practices skill.

Create an animated data dashboard video (1080x1920, 30fps, 15 seconds) visualizing this data.

SAFE ZONE: All text and key content must stay within the safe zone, at least 150px from the top and 170px from the bottom. Side margins: 60px minimum. MINIMUM FONT SIZES: Headlines 56px+, body/subtitles 36px+, labels/small text 28px absolute minimum.

## STEP 1, ANALYZE: Read the CSV file. Identify:
- A compelling title for the dashboard
- The single most impressive KPI stat (for the hero card)
- Data suitable for a bar chart (categorical comparison)
- Data suitable for a donut/pie chart (parts of a whole)
- Data suitable for a line chart (trend over time)

If the CSV doesn't have all 4 chart types, pick the best 4 visualizations and adapt. Show me the proposed dashboard layout. Wait for approval before coding.

## STEP 2, ANIMATE:

LAYOUT: Vertical stack of 4 panels with 30px padding. Top margin at 150px, bottom panel ends above 170px. Side margins: 60px. Dark background #0a0a0a.

### PANEL 1 - KPI Hero Card:
- Large number counting up from 0 with appropriate suffix (%, $, k, M)
- Trend indicator (green arrow + YoY change) slides in after count
- Glass-morphism card background

### PANEL 2 - Bar Chart:
- Horizontal bars growing from width 0 with staggered spring animations
- Labels on left, values appear at bar end after growth

### PANEL 3 - Donut Chart:
- SVG donut drawing clockwise using stroke-dashoffset
- Segments stagger, center text swaps with each segment
- Colored legend dots below

### PANEL 4 - Line Chart:
- SVG polyline drawing left to right
- Data point circles pop in as line reaches them
- Gradient fill below the line

## BACKGROUND MUSIC (REQUIRED):
1. Search Pixabay for a royalty-free lo-fi or electronic beat
2. Add using Remotion's <Audio> component with volume 0.3, must loop

This is not optional.

PREVIEW: After building, launch Remotion Studio (npx remotion studio) so I preview the video in my browser.
