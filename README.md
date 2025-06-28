# Project01
This is project-01 for lede program.
<br>
Link to the project-01 (https://akiha1224.github.io/Project1/)
<br>
Repository for data and code(https://github.com/AKIHA1224/Project1_note)

## Title
A Map of Dementia-Related Missing Persons in Japan
<br>
Based on data released by the National Police Agency

## Aim
To clearly convey trends by mapping and visualizing the number of dementia-related missing persons from 2012 to 2024—not just reporting record-high figures, but presenting the data in a way that reveals patterns across regions.

## Findings
1. While aging is often cited as one reason for the high rate of dementia-related missing persons, it became clear that in Japan, prefectures with a high aging rate (the proportion of people aged 65 and older in the total population) do not necessarily show a high rate of dementia-related missing persons.
2. The prefectures with high dementia-related missing person rates have remained largely consistent from 2012 to 2024. However, the specific reasons for these high rates have not been thoroughly analyzed at the prefectural level. During the production of this project, news reports from various regions were reviewed, but no clear explanations were found.

## Data
These are the sources for my data:

| What I plotted  | Data source |
| ------------- | ------------- |
|Number of dementia-related missing persons by prefecture in Japan|National Police Agency, 2012–2024 (PDF)|
|Total population by prefecture in Japan (2012–2024)|Portal Site of Official Statistics of Japan (e-Stat)|
|Population aged 65 and over by prefecture in Japan (2012–2024)|Portal Site of Official Statistics of Japan (e-Stat)|
|GeoJSON data of Japanese prefectures|Geospatial Information Authority of Japan (GSI)<br>https://github.com/dataofjapan/land/blob/master/japan.geojson|

## Data Collection Process
1. Convert the "Number of dementia-related missing persons by prefecture in Japan" from PDF to a CSV file. Data from 2012 to 2023 was available in a single file, while the 2024 data was released in June and was merged into the same dataset.

2. Download the "Total population by prefecture in Japan (2012–2024)" as a CSV file and combine it with the number of dementia-related missing persons to calculate the missing person rate.

3. To improve readability, calculate the dementia-related missing person rate per 100,000 people.

4. To compare with the aging rate, download the "Population aged 65 and over by prefecture in Japan (2012–2024)" and calculate the aging rate using the total population data.

## Data Analysis Process
1. Visualized the number of dementia-related missing persons per 100,000 people by prefecture from 2012 to 2024 using Flourish to show year-to-year changes.

2. Created a background map of Japan using Mapbox by combining the 2024 dementia-related missing person rates with the GeoJSON data of Japanese prefectures ([https://github.com/dataofjapan/land/blob/master/japan.geojson](https://github.com/dataofjapan/land/blob/master/japan.geojson)).

3. Calculated the number of dementia-related missing persons using pandas and visualized the results with Flourish.

4. Identified prefectures with the highest dementia-related missing person rates using pandas and created a chart showing trends of the top prefectures from 2012 to 2024.

5. Created a chart of aging rates and visualized the relationship by highlighting prefectures with high dementia-related missing person rates in red.

## New Skills and Growth
1. Although the PDF data was relatively clean, successfully converting it into a CSV file contributed to improving my pandas skills, particularly in merging CSV files.

2. Learned JavaScript in order to understand and apply scrollytelling techniques.

3. Gained knowledge of HTML and CSS, which deepened my understanding of web structure and layout.

## Future Work
During the initial stages of data cleaning, I proceeded without unifying labels such as "Region" and "Prefecture," and didn’t decide whether to use “Tokyo” or “Tokyo Metropolis.” As a result, I ended up repeating the same tasks multiple times and wasting time. Moving forward, I plan to carefully review the collected data and standardize labels from the beginning.

While I was able to use Mapbox and JavaScript to create a scrolling map experience, I wasn’t able to add enhancements such as changing colors to highlight the prefecture being discussed or adjusting the camera angle after zooming in.

I also realized that some charts may have been easier to understand if they were presented as tables instead, or if the numbers and labels had been simplified. In the future, I want to focus on creating simple, clear charts that align closely with the message I want to convey.

As I hope to continue creating pages that tell stories using maps and location-based visuals, I want to pay more attention to organizing information, citing sources properly, and conducting thorough data analysis.
