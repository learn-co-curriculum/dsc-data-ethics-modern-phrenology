# AI Phrenology and How to Avoid It

* Applications of ML and pseudoscience
* Some things cannot be measured
* Limitations of ML (emotion, gender) and proxy measurement
* Teaching data scientists scientific history

Although much of the work in statistics was done to enable “racial hygiene”, some of the pseudoscientific applications of ML are still being used and proposed today. Due to various reasons, most notably a lack of historical science education and social science being taught to engineers, we still have applications of ML arise that perpetuate many debunked pseudosciences. 

Some examples include using ML to attempt gender and emotion classification, as well as criminality based on images of human subjects. Using one’s outward appearance to predict factors like criminality are under the umbrella of phrenology, a pseudoscience which attempts to predict mental traits based on the bumps, shape, and size of one’s skull. The largest assumption this method makes is that one’s outward appearance impacts each individual’s traits. The same assumptions are made by engineers to predict traits using images and machine learning today. 

While big tech companies have developed and sell emotion and gender detection software, these tools leverage phrenology’s assumptions and are inadequate applications of machine learning. In fact, machine learning cannot detect criminality, gender, emotion, or race.

ML systems attempting to do this incorrectly measure physical attributes that are mere proxies for unobservable human phenomenon. Take emotions for example, while a smile may be an indicator of happiness, we cannot assume a smile means happiness to everyone in every context. Due to varying cultural differences, assumptions about specific facial movements cannot be applied across large populations of people. A smile is a measurable proxy, but not an emotion. People don’t always outwardly show their true emotions, and inference on what face someone is making is intrinsically tied to the assumptions of those building and annotating images. 

Emotion “detection” tools use the beliefs and assumptions of their creators to classify emotions. The range of human emotions is vast and far from universal. As data scientists, we must understand the hard limits of tools like Machine learning and where they come from. ML cannot be used to detect emotion because the data (images) don’t match the model (image classifier), but ML cannot detect emotion because physical movements are a poor proxy for true emotion. 

Although various human phenomena can’t be measured, misguided researchers still publish papers that leverage digital phrenology for criminality detection, another use case where ML fails. Without a proper education on scientific history, it’s easy to make often repeated mistakes that can harm various marginalized communities. 
