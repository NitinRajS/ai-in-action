# **Voice-to-Text (Speech-to-text)**

**Introduction to Artificial Intelligence:**

Artificial Intelligence (AI), at times called as Machine Intelligence is defined as the study of intelligent agents where any device that perceives its environment and takes actions that maximize its chance of successfully achieving its goals. The term &quot;artificial intelligence&quot; is applied when a machine mimics &quot;cognitive&quot; functions that humans associate with other human minds, such as &quot;learning&quot; and &quot;problem solving&quot;. Artificial Intelligence (AI), at times called as Machine Intelligence is defined as the study of intelligent agents where any device that perceives its environment and takes actions that maximize its chance of successfully achieving its goals. The term &quot;artificial intelligence&quot; is applied when a machine mimics &quot;cognitive&quot; functions that humans associate with other human minds, such as &quot;learning&quot; and &quot;problem solving&quot;.

**Voice-to-Text or Speech-to-Text:**

Voice is the new interface driving ambient computing. Speech recognition is transforming our daily lives from digital assistants, dictation of emails and documents, to transcriptions of lectures and meetings.

Speech recognition is the inter-disciplinary sub-field of computational linguistics that develops methodologies and technologies that enables the recognition and translation of spoken language into text. It is also known as **automatic speech recognition (ASR)**, **computer speech recognition** or **speech to text (STT)**.

Several API&#39;s are available in the cloud by various tech giants such as Microsoft, Google, IBM, etc., that convert spoken audio to text. Call the API to recognize audio coming from the microphone, from other real-time streaming audio sources, or from a recorded audio file. You can use the API to build voice-triggered smart apps.

**Uses of Speech-to-text:**

There are several areas where Speech Recognitions helps business and those are listed below:

**Automatic Transcription that saves time:**

Productivity and efficiency at all-time are top priorities when running a business with limited staff and/or resources.

By using speech recognition to convert audio and video into perfectly-accurate text, below process can be automated:

- Complaint analysis
- Call (and caller) categorization
- Repeat call analysis
- Demographic analysis
- Legal compliance
- NPS analysis

**Streamline the support process:**

Recorded audio from customer calls may just hold the answer to a better way to provide support. After taking the time to capture customer interactions and then analysing the findings, you&#39;ll be able to pinpoint the issues that people need the most help with to make the customer support process much more optimized.

**Identify callers and mitigate risk:**

With speech recognition solutions that capture audio using best-in-class voice biometrics, an organization can easily identify and authenticate each caller in order to better detect and mitigate fraud.

**Microsoft Cognitive Custom Speech API:**

Custom Speech Service from Microsoft is a cloud-based service that provides users with the ability to customize speech models for Speech-to-Text transcription. The Custom Speech Service enables you to create **customized language models** and **acoustic models** tailored to your application and your users. By uploading your specific speech and/or text data to the Custom Speech Service, you can create custom models that can be used in conjunction with Microsoft&#39;s existing state-of-the-art speech models.

For example, if you&#39;re adding voice interaction to a mobile phone, tablet or PC app, you can create a custom language model that can be combined with Microsoft&#39;s acoustic model to create a speech-to-text endpoint designed especially for your app. If your application is designed for use in an environment or by a user population, you can also create and deploy a custom acoustic model with this service.

Custom Speech Service would be useful if you expect voice queries to your application to contain particular vocabulary items, such as product names or jargon that rarely occur in typical speech, it is likely that you can obtain improved performance by customizing the language model. For example, if you were building an app to search MSDN by voice, it&#39;s likely that terms like &quot;object-oriented&quot; or &quot;namespace&quot; or &quot;dot net&quot; will appear more frequently than in typical voice applications. Customizing the language model will enable the system to learn this.

Similarly, customizing the acoustic model enables the speech recognition system to be accurate in particular environments. For example, if a voice-enabled app is aimed for use in a warehouse or factory, a custom acoustic model can accurately recognize speech in the presence of loud or persistent background noise. Customers can upload audio data with accompanying transcripts to build acoustic models.

Below is the overall flow in creating and deploying Custom Speech Service

![Custom Speech Servie Process Flow](https://github.com/NitinRajS/ai-in-action/blob/master/Voice-to-Text%20or%20Speech-to-text/images/Custome_Speech_Flow.png?raw=true)

**Develop a sample Custom Speech Service API**

In this tutorial, you will create one acoustic model and one language model that we will evaluate and test using the Microsoft Congitive Service Speech SDK

Sample Data to be used while practising the Custom Speech Service is available in the [link](https://github.com/Microsoft/Cognitive-Custom-Speech-Service/tree/master/Samples/Sample1%20-%20Biology) .

Download the sample data to your local before starting the below steps.

**Step 1: Upload the data**

In this step you will prepare the data to be uploaded on the Custom Speech to Text portal. Follow these instructions:

1. Go to https://cris.ai and login using your MSA
2. From the menu named &#39;Custom Speech&#39; click and select &#39;Adaptation Data&#39;
3. In the Adaptation Data View click &#39;Upload&#39; button.

![Dataset](https://github.com/NitinRajS/ai-in-action/blob/master/Voice-to-Text%20or%20Speech-to-text/images/Dataset.png?raw=true)

1. Type a friendly name for your data set in the box &#39;Name&#39;
2. Optionally provide a description
3. Choose the locale. It is important to note here that once the data is uploaded the locale cannot change
4. Click the &#39;Browse&#39; button associated with the transcriptions file (.txt) and select the transcription file named &quot;adaptation\_transcriptions.txt&quot; from the data you earlier downloaded
5. Click the &#39;Browse&#39; button associated with the Audio files (zip) and select the .zip file named &quot;adaptation\_acoustic\_data&quot;.
6. Click the Import button located next to the Acoustic Datasets.

The view will change back to the main &quot;Datasets&quot; view and the progress of the upload will be shown. Monitor the Status label. When it changes to completed, the data can be used.

![Dataset](https://github.com/NitinRajS/ai-in-action/blob/master/Voice-to-Text%20or%20Speech-to-text/images/Acoustic%20Dataset.png?raw=true)

Now let&#39;s do the same for the language data.

Again, Under the section &#39;Language Datasets&#39; Click the Import Button. The view will change again to that of the Language Import

1. Enter an alias name for your language data
2. Enter a description (this steo is optional)
3. Carefully select the locate
4. Click on Browse, locate and click on the dataset named &#39;LanguageAdaptationData.txt&#39;
5. Click Create and observe the new view featuring the progress of the langauge dataset upload.
6. When the status changes to complete the data can be used

**Note:** You can edit some of the details of the uploaded data such as Name and Description. Locale cannot be changed. If this is the case, then you need to upload the data again following the aforementioned process.

Now that the data is uploaded let us adapt some models.

**Step2: Adaption**

In this step we will first create a custom acoustic model followed by a language model using the data we uploaded. At the end of this step we will be ready to evaluate our newly created models.

Adaptation is carried out for acoustic and language models in separate distinct steps. One can adapt only an acoustic or a language model or both. In this tutorial we adapt both. Let us start.

1. From the menu named &#39;Custom Speech&#39; click and select &#39;Acoustic Model&#39;
2. In the Acoustic Model View click &#39;Create&#39; button
3. Provide a friendly name to the model in the Name text box
4. Optionally Provide a description
5. Pick the locale
6. Pick the baseline model you want to adapt
7. Click Create.

**Step 3: Evaluation**

We have adapted 2 models and now we are ready to evaluate them. We will evaluate them separately and we will evaluate both together. We will carry out a total of 3 evaluations. This is generally useful to understand where the biggest impact over baseline is gained. Let us start. First, we need to upload our acoustic data.

Following the process, we described for Data Import please upload the data set entitled &#39;Acoustic Test Data&#39;. Once this is completed carry out the following instructions

1. From the menu named &#39;Custom Speech&#39; click and select &#39;Accuracy Tests&#39;
2.In the Accuracy Tests View click &#39;Create&#39; button
![Accuracy Test](https://github.com/NitinRajS/ai-in-action/blob/master/Voice-to-Text%20or%20Speech-to-text/images/Accuracy_Test.png?raw=true)
3. Provide a friendly name to the model in the Name text box
4. Optionally Provide a description
5. Pick the locale
6. Pick the baseline model you want to adapt. Note here that you will immediately see all the models that have been adapted using that baseline
7. Pick the Acoustic Model we created
8. Pick the baseline language model
9. Click Create

Observe that the view changes and the status of the evaluation is indicted by the Status label. When completed the following screen shows that Word Error Rate (WER) achieved using that model against our acoustic data.

**Step 4: Deployment**

We have 2 models and we have also identified which combination of those is the best for our production system. Let us now deploy the model.

1. From the menu named &#39;Custom Speech&#39; click and select &#39;Deployments&#39;
2. Click &#39;Create&#39; button.
3. Observe the view presented. Select the locale
4. Type a friendly name for your deployment
5. Optionally provide a description
6. Select your subscription under which you want to deployment your model
7. Leave content log in as default. This will create a deployment through which all content send to the model as well as transcriptions will be logged
8. Select the base model &#39;Microsoft Conversational Model&#39;
9. Select both the acoustic and the language model we adapted.
10. Accept the terms and click &#39;Create&#39;

![Deployment](https://github.com/NitinRajS/ai-in-action/blob/master/Voice-to-Text%20or%20Speech-to-text/images/Deployment.png?raw=true)

In the screen presented you see a table with all your deployments. You can observe the locale, name, description, the date it was created, its status and a list of actions represented by 4 links. 'Delete' enables you to delete the deployment at any time. You do not lose the models or any of the work we did earlier. 'Delete' basically decommissions the deployment and stops incurring charges. In addition, you can 'Edit' the name and description fields. 'Details' show the endpoint details and finally -since we let the logging option to default- you can see an option to delete the log data. These are the audio uploaded to the endpoint as well as the transcriptions.
Now let us have a closer look on the 'Details' link.

![Deployment](https://github.com/NitinRajS/ai-in-action/blob/master/Voice-to-Text%20or%20Speech-to-text/images/Deployed.png?raw=true)

You can view here table with the endpoint details for websocket and HTTP Rest access. At the top of the table you can view also the Subscrition Key which is used to authenticate access to that endpoint.

Let us look at the endpoints in turn.

There are 2 HTTP REST APIs one for interactive mode and one for dictation which provides punctuations. These endpoints provide final results only.

There are 2 WebSocket with the .NET/Android/iOS client library endpoints which allow us to upload audio up to 15 seconds or up to 2 minutes while both supporting dictation mode

There are additionally 2 WebSocket with the .NET service library endpoints supporting either short or up to 10mins of audio while both supporting dictation mode

And finally, there are 3 WebSocket with the Speech Protocol/JavaScript WebSocket API endpoints that support the aforementioned features.

