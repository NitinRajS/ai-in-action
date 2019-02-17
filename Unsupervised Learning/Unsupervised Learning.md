**Unsupervised learning**

Let&#39;s say, you have a bunch of photos of 6 people but without information about who is on which one and you want to divide this dataset into 6 piles, each with the photos of one individual.

You have molecules, part of them are drugs and part are not but you do not know which and you are want the algorithm to discover the drugs.

**Below images helps to better understand what unsupervised learning is:**

 ![Example1: Unsupervised Leanring](https://github.com/NitinRajS/ai-in-action/blob/master/Unsupervised%20Learning/Images/example1.png)
 ![Example2: Unsupervised Learning](https://github.com/NitinRajS/ai-in-action/blob/master/Unsupervised%20Learning/Images/example2.jpeg)

**In-theory:**

Unsupervised learning is when, you only have input data (X) and no corresponding output variables. In other words, is to model the underlying structure or distribution in the data in order to learn more about the data. There are no correct answers and there is no teacher. Algorithms are left to their own devises to discover and present the interesting structure in the data.

Unsupervised learning problems can be grouped into **clustering** and **association** problems.

- **Clustering** : A clustering problem is where you want to discover the inherent groupings in the data, such as grouping customers by purchasing behaviour.
- **Association** :  An association rule learning problem is where you want to discover rules that describe large portions of your data, such as people that buy X also tend to buy Y.

Examples of unsupervised learning algorithms are:

- k-means for clustering problems.
- Apriori algorithm for association rule learning problems.

Unsupervised learning is very useful in exploratory analysis because it can automatically identify structure in data. For example, if an analyst were trying to segment consumers, unsupervised clustering methods would be a great starting point for their analysis. In situations where it is either impossible or impractical for a human to propose trends in the data, unsupervised learning can provide initial insights that can then be used to test individual hypotheses.

Dimensionality reduction, which refers to the methods used to represent data using less columns or features, can be accomplished through unsupervised methods. In representation learning, we wish to learn relationships between individual features, allowing us to represent our data using the latent features that interrelate our initial features. This sparse latent structure is often represented using far fewer features than we started with, so it can make further data processing much less intensive and can eliminate redundant features.

**Few applications listed below:**

**Visual Recognition:**

An unsupervised learner processes 10 million videos together with related textual data such as descriptions and comments. The learner models&#39; images in the videos using statistical analysis that allows it to identify visual patterns. These patterns can then be correlated with text to develop theories about the visual traits of various things. For example, such a learner might be able to build a solid model that can identify skateboards in videos. The learner is never given the right answer but can gain confidence based on many samples. Likewise, the learner will discard many models that don&#39;t appear to be correct.

**Human Behaviour:**

A learner that possesses visual highly developed visual and speech recognition capabilities could watch many television shows to learn about human behaviour. For example, a learner might be able to build a model that detects when people are smiling based on correlation of facial patterns and words such as &quot;_what are you smiling about?&quot;_

**Robotics:**

A highly developed AI that serves as a housekeeping robot develops a theory that there is usually dust under a sofa. Each week, the theory is confirmed as the robot often finds dust under sofas. Nobody explicitly tells the robot the theory is correct, but it can develop confidence in it, nonetheless.
