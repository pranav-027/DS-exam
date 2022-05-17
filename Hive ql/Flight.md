create table FlightDetails(FlightID int,Source string,Destination string, FlightRate int)
row format delimited
fields terminated by ',';

create table FlightTime(FlightID int,DepartureDate date,DepartureTime time,DepartureDelay int)
row format delimited
fields terminated by ',';

create external table FlightDetails_ext(FlightID int,Source string,Destination string, FlightRate int)
row format delimited
fields terminated by ',';

create external table FlightTime_ext(FlightID int,DepartureDate date,DepartureTime time,DepartureDelay int)
row format delimited
fields terminated by ',';

show tables;

drop table FlightDetails;

ALTER TABLE FlightTime_ext TO FlightTime_external


load data local inpath 'Path' in to table table-name

Select AVG(DepartureTime) from FlightTime  // comman might change as per condition year 2020 and i dont have that specofoc csv

