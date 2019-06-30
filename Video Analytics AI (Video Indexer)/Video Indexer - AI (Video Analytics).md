# Video Indexer (Video Analytics)

Video analytics in artificial intelligence space is the capability of automatically analysing video to recognize humans, vehicles, objects and events.

## Applications of video analytics:

**Facial recognition:**

Cameras with facial recognition software take only milliseconds to match faces from real time video with a database of previously stored images. This can used for access control, VIP identification, capture unwanted/wanted individuals. Facial recognition not only enhances security, but it can also help organizations to create better customer experience.


![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/Facial%20Recognition.png?raw=true)

**Perimeter Protection:**

As part of perimeter protection solution, the cameras can be set to detect moving persons or vehicles and warn of possible intruders in real time. Security team can visually verify what’s going on before taking an action.

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/Perimeter%20Protection.png?raw=true)


**Counting People:**

People counting is useful in many ways such as understanding how many number of customers fluctuates over time helps retailers to improve promotions. People counting is also useful at airports, museums and everywhere where detailed visitor statistics are needed.

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/Counting%20People.png?raw=true)

**License plate recognition:**

Traditional Automated License Plate recognition was costlier but it is now cheaper with video analytics. It has reduced the cost and improves the scalability. It has also enahanced its application in the areas: automating entry and exit to car parks, enabling free traffic flow on toll roads, collecting parking fees.

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/License%20Plate%20Recognition.png?raw=true)

## Azure Video Indexer:

Azure Video Indexer is a Microsoft Cognitive Services API that enables you to extract the insights from your videos as described below:

**Face detection:** Detects and groups faces appearing in the video.

**Celebrity identification:** Video Indexer automatically identifies over 1 million celebrities – such as world leaders, actors, actresses, athletes, researchers, business, and tech leaders across the globe. The data about these celebrities can also be found on various famous websites, for example, IMDB and Wikipedia.

**Account-based face identification:** Video Indexer trains a model for a specific account. It then recognizes faces in the video based on the trained model.

**Thumbnail extraction for faces ("best face"):** Automatically identifies the best captured face in each group of faces (based on quality, size, and frontal position) and extract it as an image asset.

**Visual text recognition (OCR):** Extracts text that is visually displayed in the video.

**Visual content moderation:** Detects adult and/or racy visuals.

**Labels identification:** Identifies visual objects and actions displayed.

**Scene segmentation:** determines when a scene changes in video based on visual cues. A scene depicts a single event and it is composed by a series of consecutive shots, which are semantically related.

**Shot detection:** determines when a shot changes in video based on visual cues. A shot is a series of frames taken from the same motion-picture camera.

**Black frame detection:** Identifies black frames presented in the video.

**Keyframe extraction:** Detects stable keyframes in a video.

**Rolling credits:** identify the beginning and end of the rolling credits in the end of TV shows and movies.

## Audio insights:

**Automatic language detection:** Automatically identifies the dominant spoken language. Supported languages include English, Spanish, French, German, Italian, Chinese (Simplified), Japanese, Russian, and Brazilian Portuguese Will fallback to English when the language can't be detected.

**Audio transcription:** Converts speech to text in 12 languages and allows extensions. Supported languages include English, Spanish, French, German, Italian, Chinese (Simplified), Japanese, Arabic, Russian, Brazilian Portuguese, Hindi, and Korean.

**Closed captioning:** Creates closed captioning in three formats: VTT, TTML, SRT.

Two channel processing: Auto detects, separate transcript and merges to single timeline.

**Noise reduction:** Clears up telephony audio or noisy recordings (based on Skype filters).

Transcript customization (CRIS): Trains custom speech to text models to create industry-specific transcripts.

**Speaker enumeration:** Maps and understands which speaker spoke which words and when.

**Speaker statistics:** Provides statistics for speakers speech ratios.

**Textual content moderation:** Detects explicit text in the audio transcript.

**Audio effects:** Identifies audio effects such as hand claps, speech, and silence.

**Emotion detection:** Identifies emotions based on speech (what is being said) and voice tonality (how it is being said). The emotion could be: joy, sadness, anger, or fear.

Translation: Creates translations of the audio transcript to 54 different languages.

## Audio and video insights (multi channels):

When indexing by one channel partial result for those models will be available

**Keywords extraction:** Extracts keywords from speech and visual text.

**Brands extraction:** Extracts brands from speech and visual text.

**Topic inference:** Makes inference of main topics from transcripts. The 1st-level IPTC taxonomy is included.

**Artifacts:** Extracts rich set of "next level of details" artifacts for each of the models.

Sentiment analysis: Identifies positive, negative, and neutral sentiments from speech and visual text.

## Getting Started with Video Indexer:

Open the URL: [https://vi.microsoft.com/en-us/](https://vi.microsoft.com/en-us/)

A web page will open as shown below:

**Note:** URL and webpage content may vary whenever Microsoft (or the vendor) updates the URL and webpage.

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI1.png?raw=true)

Click on **Signin** link at the top right of the web page

Select the appropriate option (shown below) in the login page, provide your login details and login to video indexer service.

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI2.png?raw=true)

The Video Indexer home page will be opened as shown below:

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI3.png?raw=true)

Click on the **Content Model Customization**:

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI4.png?raw=true)

Click on **Add Model** as shown below:

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI5.png?raw=true)

Provide the Model name as required **Happy Ambulance**

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI6.png?raw=true)

Click on the ellipse button near the model that is created and select **Add Person**

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI7.png?raw=true)

Provide the name of the person and add photo of the person as shown below:

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI8.png?raw=true)

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI9.png?raw=true)

Iterate the step (adding the person) for all the people that are required to be trained in the model.

After adding all the people required, click on the upload at the top right of the screen to upload the video to identify the people in the video.

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI10.png?raw=true)

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI11.png?raw=true)

The uploaded video will be indexed and videoindexer will identify the people based on the photos that was already added to the model.

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI12.png?raw=true)


Click on the video file shown below to see the output of the video indexer:

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI13.png?raw=true)


Once you click on the video, the output by the video indexer can be seen as shown below:

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI14.png?raw=true)

![](https://github.com/NitinRajS/ai-in-action/blob/master/Video%20Analytics%20AI%20(Video%20Indexer)/Images/VI15.png?raw=true)

