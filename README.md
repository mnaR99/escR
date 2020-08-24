# Eurovision Song Contest R

Eurovision Song Contest Web-scrapped data

# Data

# `results.csv`

|variable          |class     |description |
|:-----------------|:---------|:-----------|
|year                 |double     | Year of the event |
|events_urls          |character  | Event Information URL |
|stage                |character  | Contest Stage |
|r_o                  |double     | Running Order |
|country              |character  | Participating country |
|contestant           |character  | Artist/Band |
|song                 |character  | Name of the song |
|points               |double     | Points received |
|place                |double     | Place at the end of the stage |
|qualified            |character  | Qualified to the final stage |


# `votes.csv`

|variable          |class     |description |
|:-----------------|:---------|:-----------|
|year                 |double     | Year of the event |
|events_urls          |character  | Event Information URL |
|stage                |character  | Contest Stage |
|from                 |character  | Voting Country |
|by                   |character  | Televote/Jury |
|to                   |character  | Receiving Country |
|points               |double     | Points given |

# `event_info.csv`

|variable          |class     |description |
|:-----------------|:---------|:-----------|
|year                 |double     | Year of the event |
|date                 |date       | Date of the event |
|stage                |character  | Contest Stage |
|venue                |character  | Venue |
|city                 |character  | City |
|host_country         |character  | Host Country |
|presented_by         |character  | Presenters |
|multicamera_director |character  | Multicamera Director |
|host_broadcaster     |character  | Host Broadcaster |
|executive_supervisor |character  | Executive Supervisor |
|executive_producer   |character  | Executive Producer |
