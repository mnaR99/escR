# escR <a><img src='img/escR_hex.png' align="right" height="139" /></a>

Eurovision Song Contest web scrapped data in R.

The goal of `escR` is to provide the scores, votes and general information of each Eurovision Song Contest event.

## About Eurovision Song Contest

> The Eurovision Song Contest is organised yearly by the European Broadcasting Union (EBU), together with the Host Broadcaster and some 40 Participating Broadcasters. 
> 
> Each participating broadcaster that represents their country chooses their performer (maximum 6 people) and song (maximum 3 minutes, not released before) through a national televised selection, or through an internal selection. Each country is free to decide if they send their number-1 star or the best new talent they could find.
> 
> The winner of the Eurovision Song Contest will be chosen through 2 Semi-Finals and a Grand Final. Traditionally, 6 countries are automatically pre-qualified for the Grand Final. The so-called *Big 5* — France, Germany, Italy, Spain and the United Kingdom — and the host country. From each Semi-Final, the best 10 will proceed to the Grand Final.
> 
> After all songs have been performed, each country will give two sets of 1 to 8, 10 and 12 points; one set given by a jury of five music industry professionals, and one set given by viewers at home. Viewers can vote by telephone, SMS and through the official app.
> 
> Only those countries who take part in the respective Semi-Final vote, along with 3 of the 6 pre-qualified countries. Which countries take part and vote in which Semi-Final is determined by the so-called Semi-Final Allocation Draw in late January.
> 
> In the Grand Final, juries and viewers from all participating countries can vote again, after the 26 finalists have performed.
> 
> The winner will perform once again, and take home the iconic glass microphone trophy. The winning country will traditionally be given the honour of hosting the next Eurovision Song Contest.

## Data Dictionary

### `results.csv`

|variable          |class     |description |
|:-----------------|:---------|:-----------|
|year                 |double     | Year of the event |
|events_urls          |character  | Event Information URL |
|stage                |character  | Contest Round |
|r_o                  |double     | Running Order |
|country              |character  | Participating country |
|contestant           |character  | Artist/Band |
|song                 |character  | Name of the song |
|points               |double     | Points received |
|place                |double     | Place at the end of the stage |
|qualified            |character  | Qualified to the final stage |

### `votes.csv`

|variable          |class     |description |
|:-----------------|:---------|:-----------|
|year                 |double     | Year of the event |
|events_urls          |character  | Event Information URL |
|stage                |character  | Contest Round |
|from                 |character  | Voting Country |
|by                   |character  | Televote/Jury |
|to                   |character  | Receiving Country |
|points               |double     | Points given |

### `event_info.csv`

|variable          |class     |description |
|:-----------------|:---------|:-----------|
|year                 |double     | Year of the event |
|date                 |date       | Date of the event |
|stage                |character  | Contest Round |
|venue                |character  | Venue |
|city                 |character  | City |
|host_country         |character  | Host Country |
|presented_by         |character  | Presenters |
|multicamera_director |character  | Multicamera Director |
|host_broadcaster     |character  | Host Broadcaster |
|executive_supervisor |character  | Executive Supervisor |
|executive_producer   |character  | Executive Producer |

### `lyrics.csv`

|variable          |class     |description |
|:-----------------|:---------|:-----------|
|year                 |double     | Year of the event, 2010-2020 |
|events_urls          |character  | Event Information URL |
|country              |character  | Participating country |
|contestant           |character  | Artist/Band |
|song                 |character  | Name of the song |
|composed_by          |character  | Composers |
|written_by           |character  | Writers |
|language             |character  | Language |
|lyrics               |character  | Lyrics |
