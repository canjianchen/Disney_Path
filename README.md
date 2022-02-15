# ThemeParkOptimization
 Project to find optimal path to take for a given stay at the Disney California Adventure Park

# Introduction
Going to the theme park is fun, but they are always crowded and expensive as well, for
example, Disneyland theme park, their ticket costs at least $104 during off-peak season and as
much as $149 during peak season. This can cost up to nearly $10 per hour per person just to
be inside the park, as long as the visitor stays all day. This is a very large investment for one
day of entertainment, especially for families. In order to make a customer have a wonderful
experience whether they are going on the off-peak season or peak season.

# Minimum Viable Product:
 We come up with an idea that making a product as a website that can allow the customer to pick their destination theme park, and our product will create optimal paths for visitors at a theme park such that they could go on the rides they want while spending the least amount of time waiting in line. visitors can assign levels of satisfaction to rides throughout the park, an optimal path can be created for them using past wait time data and their desire to experience certain attractions, and this is a DIY trip planner. To do so, we need to gather walking time, waiting time, ride duration, and satisfaction data anduse it to create a graphical representation of the park and use these data to find and analyze results from the model.

# Benefits: 
Find optimal paths through the theme park rides in theme parks which improves guest
satisfaction while minimizing waiting and walking times to achieve the goal of optimizing
the Theme Park Experience. When guests followed a suggested route, they spent significantly
less time waiting in line and allowing them to play different high customer-rating rides as many
as possible.


# Process:
1. Finished the Algorithm to find the optimal path

We need to gather walking time, waiting time, ride duration and satisfaction data and used
it to create a graphical representation of the park. Through careful deliberation on the graph
structure, we frame the question as the shortest path problem, employing modified versions of
the Bellman-Ford algorithm as the main technique for finding the solution

The data collected for this project refers to differences rides at a theme park. Many of them are
not rides and some of the rides were closed for the period of data collection. Since we want to
maximize guest satisfaction while adhering to time constraints, we need to collect data relevant
to these two categories. As far as the time-related data goes, we need to find walking times
between rides, duration of rides and wait times for each ride. The values for ride duration come
from the lengths of YouTube videos that show the entirety of the ride.

To find the time it takes to walk between rides, we went to Google Maps and entered
coordinates to find all walking times between rides that don’t have other rides directly in
between them. We are then able to find the connection between any two rides in the park by
finding the shortest path given these smaller segments of time.

Wait times vary greatly throughout the day at any theme park. To collect this data, we found wait
times recorded for each ride every five minutes on thrill-data.com.

Satisfaction levels are data that are very personal and guest specific. Therefore, this data will
change based on who we are tailoring our algorithm towards. Each visitor in a group rates their
expected satisfaction of each ride from 0 to 10 where 0 indicates a ride they would really
despise going on and 10 indicates an attraction that is necessary to experience for their visit to
be complete.

To get results, we need to convert this data into a graph and to do so we will use a mostly
topographical approach

We divide the solving operation in the following steps:
– Finding the shortest walking routes to each available ride from each available ride. This allows
us to store the shortest walking times between any given pair of rides, and since walking times
are static, i.e. they don’t change with time, we do not ever need to recalculate them.

– Consider that the time from t0 to tf has M = (tf − t0) total minutes. We then restructure our
graph, now considering each vertex as M separate vertices, and find the path with highest
satisfaction, taking into account the extra constraints of shopping and eating.

constraint: Highest Satisfaction, Time Limit and Changing Wait Times, Satisfaction Decay

2. Implementing the integration of back end and front end - In Process
design:
https://www.figma.com/file/NKe5Vu2Uqr9swBYfbaLeId/UI-Design?node-id=0%3A1

So far We have implemented the basic structure and style with pure CSS/HTML

