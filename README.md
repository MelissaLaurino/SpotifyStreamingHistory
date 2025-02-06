# Spotify Streaming History
## A "Lifetime" of Spotify data and streaming history from 2012-2024

Data was extracted from account user Melissa Laurino using the Download your Data tool on [www.Spotify.com](www.Spotify.com).

It is recommended to read the documention provided by Spotify before beginning the data exploration.
- Understanding your data: <https://support.spotify.com/us/article/understanding-my-data/>

Account user: Melissa Laurino
Data subset: 2012-2024
Date of access: February 1, 2025

Data Cleaning:
- Original .json files were converted to .csv in R.
-   Data was subsetted to only include years 2012-2024, although data was downloaded in 2025.
-   Some artists and songs were removed.

Data fields, types, and definitions:
- ts - This field is a timestamp indicating when the track stopped playing in UTC (Coordinated Universal Time). The order is year, month and day followed by a timestamp in military time
- username - This field is your Spotify username.
- platform - This field is the platform used when streaming the track (e.g. Android OS, Google Chromecast).
- ms_played - This field is the number of **milliseconds** the stream was played.
- conn_country - This field is the country code of the country where the stream was played (e.g. SE - Sweden).
- Ip_addr_decrypted - This field contains the IP address logged when streaming the track.

