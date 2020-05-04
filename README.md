# dirtrally2-event-data
 
 ### Data Visualizer
 [Graph the data!](https://www.chrisraff.com/dirtrally2)
 
 
 ### How to Use This Data
Each Community Event is a JSON file in the `daily` folder. The "entries" field tells you how well each player did.

This repo is hosted on Github Sites. This means you can perform a `GET` request to get a specific stage without ever pulling the repository (which will eventually be very large). Each directory has an `info.json` file to tell you what files and directories are inside it. You can `GET` the `info.json` for the `daily` category at the URL `https://www.chrisraff.com/dirtrally2-event-data/daily/2020/info.json`. This file contains the list of available stages and all their associated metadata in the `files` array. Once you find the stage you want based on the metadata, for example `51633_51965_0.json`, you can `GET` it from the URL `https://www.chrisraff.com/dirtrally2-event-data/daily/2020/51633_51965_0.json`.

### Source

The data comes from the [Dirt Rally 2.0 Community Event page](https://dirtrally2.com/community-events). Data can only be gathered in pages of 100 players, and you need to go over an entire stage 3 times to collect which  `platform`, controller (`wheel`) and `assist`s each player used. I may eventually post that repository, but no one else should need to hit CodeMaster's servers like this since I've gone and done it for everyone.
