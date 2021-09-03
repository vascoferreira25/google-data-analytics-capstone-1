# Cleaning data

The process to clean the data is the following:

1. Check if the trip duration is correct by calculating it using the formula
   \\(\text{ended_at} - \text{started_at} > 0\\).
2. Check if there is any `usertype` missing
3. Check if there is any `station` missing
4. Even if the station is missing, keep data that has the `latitude` and
   `longitude` so we can calculate the distance traveled.
5. Calculate the distance traveled with the [Haversine
   Formula](https://en.wikipedia.org/wiki/Haversine_formula)
   
**Note:** This process will take a while to complete as it uses at least 2-3GB
RAM and the `Haversine` formula takes a while to calculate all the distances
for all the 4.3 million rows.
