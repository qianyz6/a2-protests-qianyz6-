# Assignment 1: Protests

During the past few years in the United States, there has been a surge of protests in support of the Black Lives Matter movement, women's rights, trans rights, immigration reform, gun control, the environment, and many other social and political issues.

In this assignment, you will work with data from [CountLove](https://countlove.org/), a group that collects data about protests from across the United States, including information about the purpose of the protests, the location of the protests, as well as how many people attended the protests. This data has often been [cited by the *New York Times*](https://www.nytimes.com/2020/08/28/us/black-lives-matter-protest.html), among other major outlets.

Through this assignment, you will be able to answer questions including:
- What were the most attended and least attended protests in the US in the last 5 years?
- How many protests occurred in Washington state?
- How did the number of protests in 2019 compare to 2020, and why?
- Why are people protesting in the US? What are the biggest motivators?


This assignment is divided into 2 parts. You will complete your coding work in the `analysis.R` file, and you will write short answer responses related to critical analysis and reflection of the data in this `README.md` file. Before getting started on your coding work, you should complete the section **"Critical Analysis & Reflection: Before You Code"** below.

When you are finished with the assignment, be sure to push all changes to your GitHub repository and then submit the link on Canvas.

## Before You Code: Critical Analysis & Reflection

Before diving into this (or any) dataset, it's important to know where the data came from, and it's important to have or to seek out _domain familiarity_ — in other words, knowledge about the subject/topic of the dataset. (We don't want to be "strangers in the dataset," as Catherine D'Ignazio and Lauren Klein describe it.)

To get more familiar, we are going to begin by doing some background reading.

- First, please read [this FAQ](https://countlove.org/faq.html) from the CountLove website and the opening of [this blog post](https://www.tommyleung.com/countLove/index.htm). Based on the information in these pieces, why did the creators start collecting the CountLove data? Please answer in 2-3 sentences (3 points)   
> **Because it’s easy to lose track of exactly where and when protests took place and how many people participated. Besides,keeping a record of protests can help citizens,journalists,and politicians for make efforts to a better country.**

- Next, we would like you to read this [*New York Times* piece, which uses CountLove data](https://www.nytimes.com/interactive/2020/06/13/us/george-floyd-protests-cities-photos.html) (here's a [Google Doc version for anyone who gets paywalled](https://docs.google.com/document/d/1sdjFsA5csYuH4plNEEk7WXT77K5h5ZuyW05CBwYdk6A/edit?usp=sharing)), and which describes the Black Lives Matter protests that occurred in the summer of 2020. Please summarize the main point or argument of this article in 2-3 sentences (3 points)     
>**The main point of this article is that the protests are a sign of the growing inequality in the United States, and that the police are not doing a good job of enforcing the law. This is a sign of the growing inequality in the United States, and it is a sign of the growing inequality in the United States.**

Next, we're going to look at the data.

Next, we're going to reflect about who collected this data, and what's actually inside it.

- Who collected and shared the CountLove data, and what do they do for a living? Please answer in 1-2 sentences(2 points)   
>**They are Tommy Leung and Nathan Perkins, engineers and scientists with a keen interest in civic responsibility and public policy.**

- As Klein and D'Ignazio remind us, when it comes to data, "what gets counted counts." What types of demonstrations does CountLove include in their data, and what types do they exclude? (3 points)    
>**They count public displays of protest that are not part of “regular business.” We typically do not include awareness events, commemorative celebrations, historic reenactments, fundraising events, townhalls, or political campaign rallies.**

- How and where does CountLove get their data about the protests? Please answer in 2-3 sentences (2 points)    
>**They built special software stack to crawl local newspaper and television sites on a daily basis, and most of the protest data came from these crawls.**

- How does CountLove make their estimates about the number of people who attended a protest? What potential problems might arise from this method of estimation? Please answer in 3-4 sentences (4 points)    
>**They interpret “a dozen” as 10, “dozens” as 20, “hundreds” as 100, and so forth. If an article mentions a demonstration but does not include an attendance count, they note the demonstration but leave the count empty. Inaccurate estimated number and strong reliance on the news especially when terms used for discribing the number are hundreds and thousands, and when different news use different terms to describe the same number, can lead to a lot of problems.**

- What is the purpose of the CountLove data? Please answer in 2-3 sentences (2 points)    
>**The purpose of the CountLove data is to keep a record of ongoing protests,and making the data more accessible helps citizens, journalists, and politicians make more compelling cases for a diverse, empathetic, and kind country.**

- What is the purpose of the CountLove website? Please answer in 2-3 sentences (2 points)    
>**The purpose of the CountLove website is to provide diverse comprehensive visualized pictures and tables of the protest movement in the United States.**

## While You Code: Critical Analysis & Reflection

- Reflection 1: Why do you think the mean is higher than the median? Which metric would you use in a report about this data, and why? Please answer in 2-3 sentences (2 points)      
>**The mean is higher than the median because the mean is sensitive to outliers, and the data set contains a large number of outliers.**     
>**The median is less affected by outliers, and is a better measure of central tendency for this data set.**     

- Reflection 2: Before actually calculating the number of protests that occurred in 2018, 2019, 2020, record your guesses for the following questions. (1 point)

  Guess: Do you think there were more protests in 2019 than in 2018? Why or why not? Please answer in 1 or 2 sentences      
  >**I think there were more protests in 2019 than in 2018. Because there were more controvercial societal events in 2019.**

  Guess: Do you think there were more protests in 2020 than in 2019? Why or why not? Please answer in 1 or 2 sentences     
  >**Yes,because of Covid-19 and many people's unapproval of the movements that the US government took.**
- Reflection 3: Does the change in the number of protests from 2018 to 2019 to 2020 surprise you? Why or why not? What do you think explains the fluctuation? Please answer in 1 or 2 sentences (2 points)       
>**Yes,because there are more protests in 2018 than in 2019 and which is out of my expectation. I suppose big societal events could directly affect the number of protests and it explains the fluctuation.**
- Reflection 4: What is the first and fourth most frequent category of protest? Do these frequencies align with your sense of the major protest movements in the U.S. in the last few years? Why or why not? (3 points)      
>**The first and fourth most frequent category of protest are "Racial Injustice" and "Immigration". I think they align with my sense of the major protest movements in the U.S. in the last few years. Because the protest movements in the U.S. in the last few years are "Racial Injustice" and "Immigration".**

## After You Code: Critical Analysis & Reflection

In the second chapter of *Data Feminism*, Klein and D'Ignazio describe 4 ways that data scientists can challenge power and take action:
> Taking action can itself take many forms, and in this chapter we offer four starting points:  
> (1) Collect: Compiling counterdata—in the face of missing data or institutional neglect—offers a powerful starting point as we see in the example of the DGEI, or in María Salguero’s femicide maps discussed in chapter 1.  
> (2) Analyze: Challenging power often requires demonstrating inequitable outcomes across groups, and new computational methods are being developed to audit opaque algorithms and hold institutions accountable.  
> (3) Imagine: We cannot only focus on inequitable outcomes, because then we will never get to the root cause of injustice. In order to truly dismantle power, we have to imagine our end point not as “fairness,” but as co-liberation.  
> (4) Teach: The identities of data scientists matter, so how might we engage and empower newcomers to the field in order to shift the demographics and cultivate the next generation of data feminists?  

- How does the CountLove project embody one or more of these 4 forms of challenging power? Please answer in at least 3-4 sentences (3 points)       
>**The CountLove project embodies the principles of challenging power as outlined in "Data Feminism" by engaging in the collection of counterdata, the analysis of inequitable outcomes, and the act of teaching through its methodology and goals. CountLove is collecting counterdata against the backdrop of underreported or neglected social movements. CountLove develop brand-new software stack and algrithms to analysize data, and this helps challenging powers. CountLove develop the web to let more people know the truth and pay attention to the protests, this really helps to teach many people something about data science and data feminists unconsciously.**
- What is the most interesting or surprising thing you learned from this analysis? Please answer in at least 2-3 sentences (2 points)       
>**The most interesting or surprising thing I learned from this analysis is that the number of protests is fluctuating in the last few years. And I can directly spot that there is a big difference between the number of protest in 2019 and in 2020 because of Covid-19 and many people's unapproval of the movements that the US government took.Data does tell a story.**
- What is a kind of analysis that you would like to do or that would be interesting to do with the CountLove data that you don't have the time or skills to accomplish at this moment? Please answer in at least 2-3 sentences (2 points)        
>**I think it would be interesting to do a kind of analysis that shows the difference between each state's protest number and go deeper to find out the societal reasons behind the difference. So maybe I should seek more relavant data to dig the history in each state.**