## Bike share stats data
Urbica Design analyzed the performance statistics of the city bicycle rental in 2015 for the Department of Transport of Moscow. Data on 812 000 rides at 300 rental stations were studied and analyzed taking into account each ride direction and thematic segments. See the project: [urbica.co/bikes/](http://urbica.co/bikes/)

We're publishing the aggregated data used in the project. 

The data represented in the [GeoJSON](http://geojson.org/) format

There are two datasets:

####Bike stations
The data about docking stations:
`code` docking station id
`name` station name (in Russian)
`slots` station capacity
`subway_distance` distance to the nearest subway station in meters
`district` district id (see districts)
`depertures` total count of rentals (departures) 
`arrivals` total returns (arrivals)
`in_out` departures/arrivals ratio
`roundtrips` the percentage of trips started and ended on the same station
`average` average rides (departures) count, per day
`unique_rides` percentage of unique users
`start` the date when the station started to work in the season
`start_month` the month when station started
`lat` latitude
`lon` longitude


####Directions
`source` source station code
`source_district`
`source_subway` distance to the nearest subway from the source bike station
`destination` destination station code
`destination_districts` 
`destination_subway` distance to the nearest subway from the destination bike station
`total` total rides count on this direction
`total_reverce` rides count in the opposite direction
`oneway` the ratio total/total_reverse
`is_roundtrip` is the source = destination? 
`average_duration` average duration on this route
`shortest_time` the time (not relevant, this is pedestrian time)
`average_shortest` the ratio shortest_time/average_duration
`distance` the shortest path length in meters
`fares_day` percentage of rides made on 'Day' fare
`fares_month` 'Month' fare percentage
`fares_season` 'Season' fare percentage

####Districts
`id` district id (used in stations and directions district reference)
`name` district name (Russian)
`district_rides` rides count started and ended in the stations inside the district
`average_duration` average duration time of riding for the rides in the district
`stations_count` docking stations count in the district
`total_rides` total rides started in the stations in this district
`local_rides_percent` the ratio district_rides / total_rides in percent
`name_en` district name (English)
`name_ru` district name (Russian)

## License

The data distributing under the [Creative Commons Attribution-NonCommercial license](http://creativecommons.org/licenses/by-nc/4.0/)

Attribution: 
© [Urbica Design](http://urbica.co/)
© [Velobike.ru](Urbica)


