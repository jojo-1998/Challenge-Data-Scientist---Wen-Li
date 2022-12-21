# Challenge-Data-Scientist---Wen-Li
## Work Environment
Already include `!pip install <packages>` into first code bucket in Jupter Notebook. If there are any packages missing to install, please just run:
                `!pip install <packages>`
## Assumption
(1) Des-O/Des-I denotes the destination Airport Code, which means one city may have multiple different Airport Codes.


(2) If the program(I) and operation(O) make different, then it means the flight does to be changed due to a special accident.

## Some data check codes which be removed
I removed some code to view the set of values for each variable quickly. That was for data cleaning, but they are all good, so only keep the null check since only VIO-O has one value missing.

## Features which we included in model
`avg_airline_delay`: The average delay ratio of the airline company by the current date

`avg_airport_delay`:  The average delay ratio of the destination airport by the current date

`avg_24h_delay`: The average delay ratio within last 24 hours

`is_change_flight`: The binary variable to indicate whether the flight information(either flight number or airline company) is different from program and operation

`is_change_airport`: The binary variable to indicate whether the destination airport is different from program and operation

`is_high_delay_month`: The binary variable to indicate whether the flight is scheduled in high delay rate months(7th, 12th in this case)

`is_low_delay_month`: The binary variable to indicate whether the flight is scheduled in low delay rate months(3rd, 4th in this case)

`is_Friday`: The binary variable to indicate whether the flight is scheduled in Friday

`type_N`: The binary variable to indicate whether the type of flight is national

## NOTES for reviewers
(1) The time series plot can switch to view or not view any variable in the graph by cliking the name of variable in right-top bucket. So you can see delay ratio more clear after you make count of flights and delay flights invisible.

(2) The current `avg_airline_delay`, `avg_airport_delay` and `avg_24h_delay` are not expected as my actual ideas and it will be updated once I get more time to fix bugs.
