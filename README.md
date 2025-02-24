**THE CITY OF DOGS - Data Story about NYC dogs**

**Goal**

My main goal was to make a nice story about dogs in New York and practice the workflow of a data story. In this project, I wanted to focus on using Pandas for data cleaning and building a map with Datawrapper for the first time in my life.

In this case, I’m not only a reporter but also responsible for data visualizations, photography, and webpage design. For this project, the timeframe to do all this was relatively short, given that most of these technical skills are new to me.

I chose a dataset that allowed me to build an interesting story that would be ready by the deadline. Throughout the process, I had a plan for both a maximum and a minimum version of the story. In the end, I came up with a middle-way compromise between the two.

**Tech stack used:**

Python & Pandas
HTML & CSS
Datawrapper
Process summary

**Getting the data**
NYC Health has an excellent database of dog licenses issued in the city. This is a very well-organized and clean database.

NYC Dog Licensing Dataset:
https://data.cityofnewyork.us/Health/NYC-Dog-Licensing-Dataset/nu7n-tubp/about_data

**Cleaning the data**

At first, I conducted research in Notebooks using Pandas for exploratory data analysis. My goal was to find the most interesting insights from the data. During this process, I found some issues related to dogs’ birth data. The dataset contains dogs that, according to the data, were born between 1912 and 1990 and still had a license issued in the 2020s. I emailed NYC Health to figure out how this was possible, but unfortunately, they have not yet responded.

However, since this is an official dataset run by city authorities, I didn’t let this relatively small issue ruin the whole process. That said, it did make me pivot away from visualizing the ages of NYC dogs.

Based on my analysis, I chose four different interesting angles:

Change in yearly issued licenses
Most popular breeds
Most popular names
The number of dogs in different zip codes

Here is the Notebook I mainly used for the analysis:
https://github.com/rosakettumaki/city-of-dogs-story/blob/main/dog_analysis_13022025.ipynb

**Visualizing the data**

I used Datawrapper to create the charts and a map. I decided that for the trend in issued licenses, the best way to visualize the change was a line chart.

My original idea was to use bar charts for both the most popular breeds and names and limit both charts to the top 5. But then I realized that people tend to be interested not only in the top 5 but also in how their own or their friends’ dog’s breed ranks, so I wanted to include more information. For breeds, I still wanted to keep it relatively simple and use a bar chart, so I limited it to the 15 most popular breeds. There are lots of different breeds, but the overall visualization is still manageable.

For names, I took a whole new approach and included a list of all dog names registered more than 1,000 times. At first, I did this as a bar chart, and I actually liked it. Unfortunately, Datawrapper doesn't allow search functionality in bar charts, which made me switch to a table instead. In this kind of chart, the ability to search for a specific name is crucial—rather than scrolling through a long list, you just want to know if the name you’re interested in is there or not.

For visualizing the home zip codes of these dogs, a map was the only reasonable option. I decided to create a zoomable map that first shows the overall city picture and then allows you to zoom into areas of interest.

Here are the links to the charts:

The total amount of licenses: https://datawrapper.dwcdn.net/MslE2/3/
Most popular names: https://datawrapper.dwcdn.net/Tmjm3/8/
Most popular breeds: https://datawrapper.dwcdn.net/TLFU8/3/
Map: https://app.datawrapper.de/edit/HTT02/publish

**Reporting**
I did some online research for the text, interviewed a source, and took photos at Snoot Club Pet Grooming. All the photos used in the story were taken by me at this location.

**Building the webpage**
I started by mixing two different templates and embedding my Datawrapper charts into the page. Finally, I added the photos and text.

GitHub repo: https://github.com/rosakettumaki/city-of-dogs-story
Story page: https://rosakettumaki.github.io/city-of-dogs-story/

**What did I learn? How could this be improved?**

In terms of data visualization, the biggest improvement needed is the map. Mapping the number of dogs per zip code might not be the best approach, since some areas have vastly different population sizes. A more accurate map could be created by combining this data with census data to calculate the number of dogs per person.

The overall style of the story could also be improved:

The graphics could be more refined.
The photos would benefit from some light editing.
The text could include more detailed facts.

Even thought there are multiple ways to improve, I really learned a lot about the process and how to manage the workflow. This was my second project following these guidelines, and the overall exprience was a lot smoother that at the fisrt time.
