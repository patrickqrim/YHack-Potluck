# YHack-Potluck

“Top 5 Overall Hack”, “Best Use of Google Cloud” Award, “Facebook Building Community” Award at YHack V. 2020 Hackathon.

Created by: Patrick Rim, Pranav Patil, Brandon Guo, Agnim Agarwal

Demo video: https://devpost.com/software/potluck-bys02q

## Inspiration
Over the course of the past year, one of the most heavily impacted industries due to the COVID-19 pandemic is the service sector. Specifically, COVID-19 has transformed the financial viability of restaurant models. Moving forward, it is projected that 36,000 small restaurants will not survive the winter as successful restaurants have thus far relied on online dining services such as Grubhub or Doordash. However, these methods come at the cost of flat premiums on every sale, driving up the food price and cutting at least 20% from a given restaurant’s revenue. Within these platforms, the most popular, established restaurants are prioritized due to built-in search algorithms. As such, not all small restaurants can join these otherwise expensive options, and there is no meaningful way for small restaurants to survive during COVID.

## What it does
Potluck provides a platform for chefs to conveniently advertise their services to customers who will likewise be able to easily find nearby places to get their favorite foods. Chefs are able to upload information about their restaurant, such as their menus and locations, which is stored in Potluck’s encrypted database. Customers are presented with a personalized dashboard containing a list of ten nearby restaurants which are generated using an algorithm that factors in the customer’s preferences and sentiment analysis of previous customers. There is also a search function which will allow customers to find additional restaurants that they may enjoy.

## How I built it
We built a web app with Flask where users can feed in data for a specific location, cuisine of food, and restaurant-related tags. Based on this input, restaurants in our database are filtered and ranked based on the distance to the given user location calculated using Google Maps API and the Natural Language Toolkit (NLTK), and a sentiment score based on any comments on the restaurant calculated using Google Cloud NLP. Within the page, consumers can provide comments on their dining experience with a certain restaurant and chefs can add information for their restaurant, including cuisine, menu items, location, and contact information. Data is stored in a PostgreSQL-based database on Google Cloud.

## Challenges I ran into
One of the challenges that we faced was coming up a solution that matched the timeframe and bandwidth of our team. We did not want to be too ambitious with our ideas and technology yet provide a product that we felt was novel and meaningful.

We also found it difficult to integrate the backend with the frontend. For example, we needed the results from the Natural Language Toolkit (NLTK) in the backend to be used by the Google Maps JavaScript API in the frontend. By utilizing Jinja templates, we were able to serve the webpage and modify its script code based on the backend results from NLTK.

## Accomplishments that I'm proud of
We were able to identify a problem that was not only very meaningful to us and our community, but also one that we had a reasonable chance of approaching with our experience and tools. Not only did we get our functions and app to work very smoothly, we ended up with time to create a very pleasant user-experience and UI. We believe that how comfortable the user is when using the app is equally as important as how sophisticated the technology is.

Additionally, we were happy that we were able to tie in our product into many meaningful ideas on community and small businesses, which we believe are very important in the current times.

## What I learned
Tools we tried for the first time: Flask (with the additional challenge of running HTTPS), Jinja templates for dynamic HTML code, Google Cloud products (including Google Maps JS API), and PostgreSQL.

For many of us, this was our first experience with a group technical project, and it was very instructive to find ways to best communicate and collaborate, especially in this virtual setting. We benefited from each other’s experiences and were able to learn when to use certain ML algorithms or how to make a dynamic frontend.

## What's next for Potluck
For example, we want to incorporate an account system to make user-specific recommendations (Firebase). Additionally, regarding our Google Maps interface, we would like to have dynamic location identification. Furthermore, the capacity of our platform could help us expand program to pair people with any type of service, not just food. We believe that the flexibility of our app could be used for other ideas as well.

## Built With
flask, google-cloud-sql, google-maps, html, jinja, python, sql
