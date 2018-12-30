Computer Vision
===============

Any AI system that processes visual information usually relies on computer
vision, and those capable of identifying specific objects or categorizing images
based on their content are performing image recognition.

This is incredibly important for robots that need to quickly and accurately
recognize and categorize different objects in their environment. Driverless
cars, for example, use computer vision and image recognition to identify
pedestrians, signs, and other vehicles.

Categories:
-----------

-   **Analyse an image** – Get the information about visual content found in an
    image. Use tagging, domain-specific models and descriptions in four
    languages to identify content and label it with confidence. Identify image
    types and colour schemes in pictures.

-   **Read text in images** - Detect text in an image using optical character
    recognition (OCR) and extract the recognised words into a machine-readable
    character stream. Analyse images to detect embedded text, generate character
    streams and enable searching. Save time and effort by taking photos of text
    instead of copying it.

-   **Read handwritten text from images** - Detect and extract handwritten text
    from notes, essays, letters, whiteboards, forms and other sources. Reduce
    paper clutter and be more productive by taking photos of handwritten notes
    instead of transcribing them and make the digital notes easy to find by
    implementing search. Handwritten OCR works with different surfaces and
    backgrounds, such as white paper, yellow sticky notes and whiteboards.

-   **Recognise celebrities and landmarks** – Recognise the celebrities from
    business, politics, sports and entertainment as well as natural and man-made
    landmarks from around the world.

-   **Analyse Video -** Use any of the Computer Vision APIs with your video
    files by extracting frames of the video from your device and then sending
    those frames to the API calls of your choice. Get results from your videos
    more quickly

-   **Content Moderation -** Easily moderate content and detect inappropriate
    content from your crowd-sourced images.

Many of the use cases of computer vision fall into the following clusters:

Banking
-------

While most of the coverage of AI in banking has involved fraud detection and
natural language processing, some computer vision technology has also found its
way into the banking industry as well

Mitek Systems offers image recognition applications that use machine learning to
classify, extract data, and authenticate documents such as passports, ID cards,
driver’s licenses, and checks.

The applications work by having customers take a photo of an ID or a paper check
using their mobile device and send to the user’s bank where computer vision
software on the bank’s side verifies authenticity. Once verified and accepted by
the user’s bank, the application or check is processed. For deposits, funds
typically become available to the customer within a business day, according to
the Mitek company website.

![](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/Banking.png)

Automotive
----------

Near half of road causalities are “**Vulnerable road users**” - pedestrians,
cyclists and motorcyclists. According to research, there’s a clear theme to most
of these incidents: human error and inattention. One of a company that claims to
make driving safer is Waymo (formerly known as Google self-driving car project).
Waymo is working to improve transportation for people, building on self-driving
car and sensor technology developed in Google Labs.

The company website reports that Waymo cars are equipped with sensors and
software that can detect 360 degrees of movements of pedestrians, cyclists,
vehicles, road work and other objects from up to three football fields away. The
company also reports that the software has been tested on 7 million miles of
public roads to train its vehicles to navigate safely through daily traffic.

![Related image](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/Self_Driving.jpg)

![Image result for waymo self driving](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/image006.0.gif)

Retail
------

Sometimes you see something you want to buy, but have no information about it.
In that case, a tool called Lens can help. It’s been launched by the photo
sharing website Pinterest as a beta product, and it could aid the in-store
experience. It works by recognizing the object and providing contextual
information about it. Perhaps it’ll tell you who designed the piece of furniture
in what year, or it’ll suggest other clothing that’ll go with a certain pair of
shoes. Just take a photo of the item, and the app does the rest.

A popular retail company uses facial recognition to identify loyalty members as
they walk into the store. CV then enables a personalized shopping experience: by
scouring their purchasing history and preferences, the system can make
personalized product recommendations specific to each shopper. By treating them
as individuals – and more importantly, as VIPs – the system instils brand
loyalty, and converts occasional shoppers into regular customers. Both of which
are good for business.

Agriculture
-----------

Some farms are beginning to adopt computer vision technology to improve their
operations. Research suggests that these technologies aim to help farmers adopt
more efficient growth methods, increase yields, and eventually increase profit.

Slantrange claims to offer computer vision-equipped drones that are connected to
what the company calls an “intelligence system” consisting of sensors,
processors, storage devices, networks, an artificial intelligence analytics
software and other user interfaces to measure and monitor the condition of
crops. At 120 meters above ground level, the camera has a resolution of 4.8
cm/pixel. However, its website notes that flying lower provides better
resolution.

The company claims that the drone captures images of the fields to show the
different signatures of healthy crops compared with “stressed” crops. These
stressors include pest infestations, nutrient deficiencies and dehydration; and
metrics to estimate potential yield at harvest, and others. These signatures are
passed on to the SlantView analytics system which interprets the data and
ultimately helps farmers make decisions related to treatment for stress
conditions.

![](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/Agriculture.png)

Security
--------

Computer Vision Artificial Intelligence plays a vital role in Security systems
and its related devices. Uber is using driver selfies to enhance security. Uber
is using Microsoft Cognitive Services to offer Real-Time ID Check. Drivers
verify their identity using selfies before they are able to accept rides.

![Uber is rolling out a new security feature](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/uber_selfie.jpg)

**Microsoft Cognitive Services – Custom Vision API**

The Custom Vision Service enables organizations to develop domain-specific
image-classification models and use it to analyse image content. Examples
include identifying a dog's breed from a picture of the dog, and identifying
defective parts produced by manufacturing processes. It was recently used to
help search-and-rescue drones identify objects such as boats and life vests in
large bodies of water and recognize potential emergency situations in order to
notify a rescue squad without waiting for human intervention.

The Custom Vision Service exposes two APIs

-   Custom Vision Training API

-   Custom Vision Prediction API

You can build, train, and test image-classification models using the Custom
Vision Service portal, or you can build, train, and test them using the Custom
Vision Training API. Once a model is trained, you can use the Custom Vision
Prediction API to build apps that utilize it. Both are REST APIs that are easily
called from a variety of programming languages.

**Try out Custom Vision API**

This part of the article will show you how to create, train and test the Custom
Vision Service model

In order to try out the Custom Vision API, below are the pre-requisite

-   A Microsoft Account

-   Microsoft Visual Studio Code version 1.14.0 or higher

Download a Zip file containing the resources from the
[link](https://a4r.blob.core.windows.net/public/cvs-resources.zip)

*Create a Custom Vision Service project*

The first step in building an image-classification model with the Custom Vision
Service is to create a project. In this exercise, you will use the Custom Vision
Service portal to create a Custom Vision Service project.

1.  Open the [Custom Vision Service portal](https://www.customvision.ai/) in
    your browser. Then click Sign In

![](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/Custom_Vision_Signin.PNG)

>   portal-sign-in.png

1.  If you are asked to sign in, do so using the credentials for your Microsoft
    account. If you are asked to let this app access your info, click Yes, and
    if prompted, agree to the terms of service.

2.  Click New Project to create a new project

    ![Creating a Custom Vision Service project](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects.PNG)

3.  In the "New project" dialog, name the project "Artworks," ensure that
    General is selected as the domain, and click Create project.

>   **Note:** A domain optimizes a model for specific types of images. For
>   example, if your goal is to classify food images by the types of food they
>   contain or the ethnicity of the dishes, then it might be helpful to select
>   the Food domain. For scenarios that don't match any of the offered domains,
>   or if you are unsure of which domain to choose, select the General domain

![](media/https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_2.PNG)

>   Creating a Custom Vision Service project

>   The next step is to upload images to the project and assign tags to those
>   images to classify them

>   *Upload Tagged Images*

>   In this exercise, you will add images of famous paintings by Picasso,
>   Pollock, and Rembrandt to the Artworks project, and tag the images so the
>   Custom Vision Service can learn to differentiate one artist from another.

1.  Click Add images to add images to the project.

![](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_3.PNG)

>   Adding images to the Artworks project

1.  Click Browse local files.

![Browsing for local images](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_4.PNG)

1.  Browse to the "Artists\\Picasso" folder in the resources that you downloaded
    earlier (from the
    [link](https://a4r.blob.core.windows.net/public/cvs-resources.zip)), select
    all of the files in the folder, and click Open.

![Selecting an image](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_5.PNG)

1.  Type "painting" (without quotation marks) into the Add some tags... box.
    Then click + to assign the tag to the images.

![Adding a "painting" tag to the images](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_6.PNG)

1.  Repeat Step 4 to add a "Picasso" tag to the images.

2.  Click Upload 7 files to upload the images. Once the upload has completed,
    click Done.

    ![Uploading tagged images](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_7.PNG)

3.  Confirm that the images you uploaded appear in the portal, along with the
    tags assigned to them.

![The uploaded images](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_8.PNG)

1.  With seven Picasso images, the Custom Vision Service can do a decent job of
    identifying paintings by Picasso. But if you trained the model right now, it
    would only understand what a Picasso looks like, and it would not be able to
    identify paintings by other artists.

2.  The next step is to upload some paintings by another artist. Click Add
    images and select all of the images in the "Artists\\Rembrandt" folder in
    the lab resources. Tag them with the labels "painting" and "Rembrandt" (not
    "Picasso"), and upload them to the project.

![Selecting an existing tag](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_9.PNG)

1.  Confirm that the Rembrandt images appear alongside the Picasso images in the
    project, and that "Rembrandt" appears in the list of tags.

![Picasso and Rembrandt images](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_10.PNG)

1.  Now add paintings by the enigmatic artist Jackson Pollock to enable the
    Custom Vision Service to recognize Pollock paintings, too. Select all of the
    images in the "Artists\\Pollock" folder in the lab resources, tag them with
    the terms "painting" and "Pollock", and upload them to the project.

With the tagged images uploaded, the next step is to train the model with these
images so it can distinguish between paintings by Picasso, Rembrandt, and
Pollock, as well as determine whether a painting is a work by one of these
famous artists

*Train the model*

1.  Click the Train button at the top of the page to train the model. Each time
    you train the model, a new iteration is created. The Custom Vision Service
    maintains several iterations, allowing you to compare your progress over
    time.

![Training the model](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_11.PNG)

1.  Wait for the training process to complete. (It should only take a few
    seconds.) Then review the training statistics presented to you for iteration
    1. Precision and recall are separate but related measures of the model's
    accuracy. Suppose the model was presented with three Picassos and three Van
    Goghs, and that it correctly identified two of the Picassos as "Picasso"
    images, but incorrectly identified two of the Van Goghs as Picassos. In this
    case, the precision would be 50% (two of the four images it classified as
    Picassos are actually Picassos), while its recall would be 67% (it correctly
    identified two of the three Picasso images as Picassos)

    ![Results of training the model](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_12.PNG)

Now let's test the model using the portal's Quick Test feature, which allows you
to submit images to the model and see how it classifies them using the knowledge
gained from the training images.

*Test the Model*

You don't have to write an app to test the model; you can do your testing in the
portal, and you can further refine the model using the images that you test
with. In this exercise, you will test the model's ability to identify the artist
of a painting using test images provided for you.

1.  Click Quick Test at the top of the page

![Testing the model](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_13.PNG)

1.  Click Browse local files, and then browse to the "Quick Tests" folder in the
    lab resources. Select PicassoTest_01.jpg, and click Open

![Selecting a Picasso test image](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_14.PNG)

1.  Examine the results of the test in the "Quick Test" dialog. What is the
    probability that the painting is a Picasso? What is the probability that it
    is a Rembrandt or Pollock?

2.  Close the "Quick Test" dialog. Then click Predictions at the top of the
    page.

![Viewing the tests that have been performed](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_15.PNG)

1.  Click the test image that you uploaded to show a detail of it. Then tag the
    image as a "Picasso" by selecting Picasso from the drop-down list and
    clicking Save and close.

![](https://github.com/NitinRajS/ai-in-action/blob/master/Computer%20Vision/CV_My_Projects_16.PNG)

>   Tagging the test image

1.  Perform another quick test using the file named FlowersTest.jpg in the
    "Quick Test" folder. Confirm that this image is assigned a low probability
    of being a Picasso, a Rembrandt, or a Pollock

The model is trained and ready to go and appears to be adept at identifying
paintings by certain artists. Now let's go a step further and incorporate the
model's intelligence into an app.
