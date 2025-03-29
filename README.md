# M-Emoji Dataset

M-Emoji is the first dataset exclusively composed of real-time emoji chat data from music-listening experiences. 

It comprises 15,795 real-time chat messages containing emojis, collected from 192 music performances by 84 different artists on YouTube.


## Dataset Overview

This dataset consists of 15,795 live chat messages containing emojis, collected from 192 songs performed by 84 artists. The dataset includes 192 individual CSV files corresponding to each song and one metadata XLSX file that provides information for all songs.

We collected live chat data from "Live chat replay" in YouTube videos released as "Premieres".

The two Youtube series selected are as follows:

- **Tiny Desk Concert** from NPR Music channel
- **A COLORS SHOW** from COLORS channel


## Folder Structure

```
M-Emoji-Dataset/
├── Emoji chat data/
│   ├── chat_0.csv
│   ├── chat_1.csv
│   ├── ...
│   └── chat_191.csv
├── Metadata.xlsx
└── README.md
```


## Files Description

### Emoji Chat Data
- Timestamp: Original chat timestamp (based on the full video timeline).
- Timestamp (seconds): Timestamp converted into seconds.
- Username: Anonymized username.
- Chat: Content of the chat message.
- Chat type: Categorized as EO (Emoji Only) for messages containing only emojis, and ET (Emoji with Text) for messages containing both emojis and text.
- Used emojis: A list of unique emojis appearing in the chat message (duplicates removed).
- Emoji count: Total number of emojis in the message, including duplicates.

### Metadata.xlsx
- Index: A unique identifier for each song (ranging from 0 to 191).
- Song title: Song title based on the original YouTube video.
- Artist: Artist name based on the original YouTube video.
- Start time: Timestamp at which the song begins within the video.
- End time: Timestamp at which the song ends within the video.
- Start time (seconds): Start time converted into seconds.
- End time (seconds): End time converted into seconds.
- Duration: Total duration of the song in seconds.
- Video ID: YouTube video ID of the source video.
- Video URL: URL of the source video.

## Use Cases

- Predicting or generating emoji reactions based on audio features
- Temporal emotion tracking over music
- Emoji-based music tagging
