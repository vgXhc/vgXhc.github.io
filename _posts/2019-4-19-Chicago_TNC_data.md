---
layout: post
title: Playing around with Chicago's Transportation Network Company dataset
---

Chicago has made available a huge dataset of rideshare data from Uber and Lyft on their Open Data portal: [https://data.cityofchicago.org/Transportation/Transportation-Network-Providers-Trips/m6dm-c72p] The data captures over 17 million individual rides, including information about start and end location, distance, time, and fares.

I downloaded the full dataset and started playing around with it.

# Trip length

One amazing thing about the trip data is the trip length. I would have expected there to be many short trip. But it was surprising to see that if you plot the number of trips by distance, the most number of trips are in the 1-mile range. Also interesting to note: The little bump at 18 to 19 miles -- that's the distance from downtown to O'Hare Airport! (I combined all trips of 30 miles and more into one bin to make the graph more meaningful)

![Trips by distance](/images/Trip Distance.svg)

# Trip hour
Another question is when trips occur in the day. Here's the number of trips by hour of the day:

![Trips by time of day (total)(/images/Trips_time_of_day_total.svg)

Because weekday and weekend travel are probably different, it makes sense to look at them separately: 

![Trips by time of day (weekday only)](/images/trips_time_of_day_weekday.svg)

![Trips by time of day (weekend only)](/images/trips_time_of_day_weekend.svg)

On weekdays, there is a pronounced morning rush peak, and then an much bigger pm rush peak; but even after rush hour, there are lot of trips all the way until midnight.

On weekends, things ramp up quickly to peak at 6 pm, stay fairly constant, and then have an even larger spike at midnight to 1 am.
