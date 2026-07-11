Task 1: Data Visualization with Tableau
What I learned: How to visualize clusters of data using Tableau. Turning raw data into charts makes it much easier to spot patterns and actually understand what's going on, instead of staring at rows of numbers.
What the task involved:

Analyzing a client's raw data
Building a dashboard from it

What I did: I imported and unified the JSON telemetry data in Tableau, created a calculated field to flag "unhealthy" machine statuses, and built bar charts comparing breakdowns across factories and across machine types. I linked the two charts with a filter so clicking on a factory would show its specific breakdown pattern by machine type.

Key Findings –

1. Factory with most downtime: Daikibo Factory Seiko (~490 unhealthy events — tallest bar in the chart)
2. Clicking into daikibo-shenzhen, I found that the LaserCutter was responsible for the vast majority of that factory's breakdowns.