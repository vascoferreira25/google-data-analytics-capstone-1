# Merging data

As the data is split into several files, the first step to make sense of the
data is to merge it into a single file.

The original data looked like this:

| ride_id          | rideable_type | started_at          | ended_at            | start_station_name           | start_station_id | end_station_name            | end_station_id | start_lat | start_lng | end_lat | end_lng  | member_casual |
|------------------|---------------|---------------------|---------------------|------------------------------|------------------|-----------------------------|----------------|-----------|-----------|---------|----------|---------------|
| A847FADBBC638E45 | docked_bike   | 2020-04-26 17:45:14 | 2020-04-26 18:12:03 | Eckhart Park                 | 86               | Lincoln Ave & Diversey Pkwy | 152            | 41.8964   | -87.661   | 41.9322 | -87.6586 | member        |
| 5405B80E996FF60D | docked_bike   | 2020-04-17 17:08:54 | 2020-04-17 17:17:03 | Drake Ave & Fullerton Ave    | 503              | Kosciuszko Park             | 499            | 41.9244   | -87.7154  | 41.9306 | -87.7238 | member        |
| 5DD24A79A4E006F4 | docked_bike   | 2020-04-01 17:54:13 | 2020-04-01 18:08:36 | McClurg Ct & Erie St         | 142              | Indiana Ave & Roosevelt Rd  | 255            | 41.8945   | -87.6179  | 41.8679 | -87.623  | member        |
| 2A59BBDF5CDBA725 | docked_bike   | 2020-04-07 12:50:19 | 2020-04-07 13:02:31 | California Ave & Division St | 216              | Wood St & Augusta Blvd      | 657            | 41.903    | -87.6975  | 41.8992 | -87.6722 | member        |
| 27AD306C119C6158 | docked_bike   | 2020-04-18 10:22:59 | 2020-04-18 11:15:54 | Rush St & Hubbard St         | 125              | Sheridan Rd & Lawrence Ave  | 323            | 41.8902   | -87.6262  | 41.9695 | -87.6547 | casual        |

The final data has around 4.3 million rows.

