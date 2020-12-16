# python_api_analysis

Please note the following points of interest below regarding this assignment:
1.	WeatherPy script pulls data from either a CSV file OR the required API and is intended for the purpose of saving incoming response rate redundancy and added flexibility. In addition, data is retrievable daily that is adjustable as needed. Before running the notebook, ensure the following parameters are met. By default, it is retrieving data from API sources on the current day. For all weather information, temperature is retrieved in unit Fahrenheit. 

a.	Insert api_keys.py file with pertinent API key information
b.	Source is set to all lowercase ‘api’ or ‘csv’ that is commented out, or uncomment for csv import
c.	Change unit to ‘metric’ for Celsius conversion
d.	CSV import on a specific day, set both ‘date’ and ‘datef’ to desired date (be the same) in the format provided that is commented out (note the format difference: date=’mm/dd/yy’ and datef=’mmddyy’ without the slashes). The datef is set to ensure proper folder and file naming convention for stored images.  
e.	One important caveat is the script does not create subfolders in either methods of data source. Ensure the subfolder is created within the ‘images’ folder and its name is consistent with datef. Again, by default datef is set to current day in the proper format as noted.
f.	Script begins at the ‘Call Defined Functions’ section during initial run
g.	The API method also exports data retrieved into separate folder called ‘data’ and each filename includes the default datef variable (e.g. wx_cities_091720.csv).  

2.	VacationPy script pulls data from both the CSV file saved above AND the required API source. In addition, data is retrievable daily and hotel information stored hourly that is adjustable as needed. Before running the notebook, ensure the following parameters are met. By default, it is retrieving data from both CSV and API sources on the current day. For ideal weather conditions and as per required instructions, temperature range is set between 70-80 degrees Fahrenheit, wind speeds less than 10mph, and cloudiness less than or equal to 0%. Radius for hotel search is set at 5000 meters around cities with ideal weather conditions. 

a.	Insert api_keys.py file with pertinent API key information
b.	As in the above section, datef is used for retrieving saved CSV file and for storing the hotel information, and by default is set to current day. For specific a day, uncomment this section and set both ‘date’ and ‘datef’ as desired (be the same but in the proper format).
c.	Hour is implemented for storing hotel data but is only used as the current hour on each API call. Placed in the subfolder ‘hotels’ within the ‘date’ folder. Notice the filename distinguishes between ideal weather conditions after the hour to provide greater flexibility when calling API within the same hour as needed.  
d.	Update ideal weather conditions as desired in the second section of ‘…fitting weather criteria’
e.	Update radius for hotel search as desired in the second section of ‘hotel map’
f.	Heatmaps are generated and can be manually saved by clicking on the left icon above the map or a screen capture. These files are stored in ‘images/heatmap/{hour}’ folder by day and hour.

3.	All charts and graphs as mentioned above are stored in images folder and the subfolders need to be manually created for each day and hour in the proper naming convention as shown.

4.	Report is available in the analysis folder, including a correlation and overall summary tables per days observed.
