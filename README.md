# Youtube-Transcript Summarizer

## About

***This project basically aims at providing clean and concise summary of the YouTube videos that the user don’t want to waste their time at.
User have to activate the app by clicking the activate button and then the URL of the video to which he/she wants to get the summary. After clicking the Transcript button, summary of the particular video has created and based on the user comfort language he/she can translate the summary  to its requirement. 
There is a feature of speech by which user can listen the audio voice of the summary in case he/she is not interested in reading.
Whole working depends on the two-working scenario:***
* Login to the app
* Summarize the video

## Work Flow of an API

![image](https://user-images.githubusercontent.com/75423160/211209469-ec987fc8-e423-43c4-bcb9-fb9ff78d7515.png)
* Input the valid YouTube video URL from the user. The First step is to getting the video link from the user which user wants to summarize. The video should be Recorded, it should have a valid video id and it should be available on YouTube. These are some of the things that user should keep in mind before using this web application.
* Getting the transcripts from that video. After taking the video link from the user, the next part is to get the transcripts on video. Now it will check whether the given video has subtitles available or not. If the Given video has subtitles in it then we can simply use the python library called YouTube_Transcript_Api which is used to extract the transcripts from the given video. Now what if the given video doesn't have subtitles in it so in this case we will first convert the video into audio format like .mp3 or .mp4 format using python library called pytube and then download that audio file. After downloading the audio file, there is a need to convert it into .wav file using ffmpeg and then doing its audio Transcription using Speech Recognition Library and Hugging sound Library. It will basically convert that audio file into text file which contains the Transcription of the video.

## popular libraries uses

```
Hugging-face,
 Speechrecognitonapi,
 tkinter(GUI),
 transformers,
 datetime,
 MBartForConditionalGeneration, 
 PIL etc. 
```

## Overview

* Activate the app.

![image](https://user-images.githubusercontent.com/75423160/211209580-08df9848-a616-450f-be3f-79795d954ee4.png)

* Enter the URL of the valid link

![image](https://user-images.githubusercontent.com/75423160/211209596-237f2e2a-0c4f-48c9-9079-62a831f5825c.png)

* Summarize the video .

![image](https://user-images.githubusercontent.com/75423160/211209625-96d160e5-a17a-4646-b9e9-d3ac153e4d13.png)

* Get the text as per your language comfort with audio facility.

![YouTube Transcript summarization](https://user-images.githubusercontent.com/75423160/211209774-797d35d9-fc59-4724-90b2-019711c19363.png)
