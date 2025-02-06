# Spotify Streaming History
## A "Lifetime" of Spotify data and streaming history from 2012-2024

Data was extracted from account user Melissa Laurino using the Download your Data tool on [www.Spotify.com](www.Spotify.com).

It is recommended to read the documention provided by Spotify before beginning the data exploration.
- Understanding your data: <https://support.spotify.com/us/article/understanding-my-data/>

Account user: Melissa Laurino <br>
Data subset: 2012-2024 <br>
Date of access: February 1, 2025 <br>

Data Cleaning:
- Original .json files were converted to .csv in R.
-   Data was subsetted to only include years 2012-2024, although data was downloaded in 2025.
-   Some artists and songs were removed.

Data fields, **types**, and definitions:
- ts - This field is a **timestamp** indicating when the track stopped playing in UTC (Coordinated Universal Time). The order is **year**, **month** and **day** followed by a **timestamp** in **military tim**e
- username - This field is your Spotify username.
- platform - This field is the platform used when streaming the track (e.g. Android OS, Google Chromecast).
- ms_played - This field is the number of **milliseconds** the stream was played.
- conn_country - This field is the country code of the country where the stream was played (e.g. SE - Sweden).
- Ip_addr_decrypted - This field contains the IP address logged when streaming the track.
- user_agent_decrypted - This field contains the user agent used when streaming the track (e.g. a browser, like Mozilla Firefox, or Safari)
- master_metadata_track _name - This field is the name of the track.
- master_metadata_album_artist_name - This field is the name of the artist, band or podcast.
- master_metadata_album_album_name - This field is the name of the album of the track.
- spotify_track_uri - A Spotify URI, uniquely identifying the track in the form of “spotify:track:<base-62 string>”
A Spotify URI is a resource identifier that you can enter, for example, in the Spotify Desktop client’s search box to locate an artist, album, or track.
- episode_name - This field contains the name of the episode of the podcast.
episode_show_name - This field contains the name of the show of the podcast.
- spotify_episode_uri - A Spotify Episode URI, uniquely identifying the podcast episode in the form of “spotify:episode:<base-62 string>”
A Spotify Episode URI is a resource identifier that you can enter, for example, in the Spotify Desktop client’s search box to locate an episode of a podcast.
- reason_start - This field is a value telling why the track started (e.g. “trackdone”)
- reason_end - This field is a value telling why the track ended (e.g. “endplay”).
- shuffle - This field has the value True or False depending on if shuffle mode was used when playing the track.
- skipped - This field indicates if the user skipped to the next song
- offline - This field indicates whether the track was played in offline mode (“True”) or not (“False”).
- offline_timestamp - This field is a **timestamp** of when offline mode was used, if used.
- incognito_mode - This field indicates whether the track was played during a private session (“True”) or not (“False”).

