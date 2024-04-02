# Youtube Watch History Exploratory Analysis
## Objective
Exploratory Data Analysis on my own Youtube History. In this project, I was able to determine:
1. Most viewed channels
2. Most watched videos
3. Video title keywords that appeared the most in the watch history (using NLP)
4. Most active hours spent watching videos throughout the day
5. Video watching patterns based on month, day, and hour of videos watched

## Technology
Language: Python

## Dataset
Own Youtube watch history obtained through Google Takout

## Data Preparation

Examining dataset to see which columns are needed

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/f5004b24-37f3-4bcd-b8c4-76867a410291)
![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/0c12090d-78ca-48f3-a3a7-0f2f7f1f0bcb)

Removed unnecessary columns

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/1c98c488-ea55-4eff-ba5e-65d210fd7e09)

Formatted 'title' column to remove the action "Watched" before all videos. Formatted 'titleUrl' to remove youtube link

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/0d37aa9f-6430-45b9-ba0d-0d3eff463207)

Obtained channel name from 'subtitles' column

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/552eeed0-e7cb-4451-8428-aedb9bb8cfd2)

Clean time column of unnecessary strings

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/6bef1f5c-0ed5-42d1-8bc6-377667ead297)

Removed columns with no channel name, as this means the video is no longer available for viewing on Youtube (i.e., either deleted or made private).

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/181aa31e-8724-40c2-aee9-310f558cf6cf)

New column made to signify if video watched was classified as the new youtube feature "Shorts"

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/f7063ae5-3c2e-4371-ae68-bfe882f2508d)

Time column used to make different columns: 'year', 'month', 'hour', 'day', 'minute'

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/b6528316-3018-44de-b872-3cf2f458eb8a)

## Exploratory Data Analysis
Data is from October 2021 to April 2024

Most viewed channels

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/de2de52f-12a9-49d0-bd80-9f47305d1dac)

Most watched youtube videos

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/6b9b864f-215e-4c9f-8bcb-33cf4fef8987)

Videos watched per hour

Overall video watching peaked at 9AM and was the lowest at 8PM

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/8b6046d0-bd45-413d-932e-047822779114)

Videos watched per day

Most videos were watched on Mondays

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/105ccb91-0da7-46e8-a165-c5ebf863790d)

Videos watched over days and hours

Overall video watching was most frequent on Mondays at 9AM and 2PM.

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/f91f8255-235e-469d-96a4-27ef6c1721db)

Videos watched over hours and months

The most videos were watched on December at 6AM over the years.

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/9715b453-b29f-4a34-aa42-d6bf3cbb5c9b)

Videos watched over days and months

Most videos were watched on Mondays of January months.

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/2aaf66a4-84a4-435f-8e2a-e27f6cf114f4)

### Natural Language Processing
Preprocessing of video titles for analysis

Functions made for text preprocessing, which included: making all words lowercase, expanding contractions, removing punctuation marks, removal of emojis, tokenization, and lemmatization. Another function made to convert list made from previous function into string. 

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/23f77ad3-4e77-4215-a129-0e9ad4056a3c)
  
![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/5312ea5e-32e9-45dd-9dab-603bc7369cec)

Word Cloud

Most watched keywords contain:

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/d7d38769-47b4-444d-854a-82e9fa8c6bd6)


Specific count of words:

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/672111b9-3323-4d40-87fe-f14f34d1f72f)

![image](https://github.com/ysasamson/YoutubeHistory/assets/145044637/93c6fdc5-c429-4721-a534-3ba152753282)
