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
Protests is a way of communication between citizens and elected officials.But lack of data of aggregate protest data make it hard to understand single protest.
- Next, we would like you to read this [*New York Times* piece, which uses CountLove data](https://www.nytimes.com/interactive/2020/06/13/us/george-floyd-protests-cities-photos.html) (here's a [Google Doc version for anyone who gets paywalled](https://docs.google.com/document/d/1sdjFsA5csYuH4plNEEk7WXT77K5h5ZuyW05CBwYdk6A/edit?usp=sharing)), and which describes the Black Lives Matter protests that occurred in the summer of 2020. Please summarize the main point or argument of this article in 2-3 sentences (3 points)
A police brutality against Floyd, a black man, has exploded the issue of racism. People everywhere in US are marching to protest this injustice
Next, we're going to reflect about who collected this data, and what's actually inside it.

- Who collected and shared the CountLove data, and what do they do for a living? Please answer in 1-2 sentences(2 points)
Tommy Leung and Nathan Perkins collected and shared the data. They want to helps citizens make more compelling cases for a kind country
- As Klein and D'Ignazio remind us, when it comes to data, "what gets counted counts." What types of demonstrations does CountLove include in their data, and what types do they exclude? (3 points)
They count public displays of protest that are not part of “regular business.” They typically do not include awareness events, commemorative celebrations, historic reenactments, fundraising events, townhalls, or political campaign rallies.
- How and where does CountLove get their data about the protests? Please answer in 2-3 sentences (2 points)
They crawl local newspaper and television sites on a daily basis. Some of data are from Crowd Counting Consortium.
- How does CountLove make their estimates about the number of people who attended a protest? What potential problems might arise from this method of estimation? Please answer in 3-4 sentences (4 points)
They record the most conservative attendance number from the news articles.  interpret “a dozen” as 10, “dozens” as 20, “hundreds” as 100, and so forth. The potential problems is that the data from newspaper is underestimated in this way.
## While You Code: Critical Analysis & Reflection

- Reflection 1: Why do you think the mean is higher than the median? Which metric would you use in a report about this data, and why? Please answer in 2-3 sentences (2 points)
The mean is higher than the median because the max of attendees is much larger than other data. I would use median in a report about this data because the influence of the largest data is less on median than on mean.
- Reflection 2: Before actually calculating the number of protests that occurred in 2018, 2019, 2020, record your guesses for the following questions. (1 point)

  Guess: Do you think there were more protests in 2019 than in 2018? Why or why not? Please answer in 1 or 2 sentences
I believe there were more protests in 2019 than in 2018 because when the issue of racism get more serious, it's more possible to be a event that attract the public's attention.
  Guess: Do you think there were more protests in 2020 than in 2019? Why or why not? Please answer in 1 or 2 sentences
I believe there were more protests in 2020 because George Floyd died this year which brought attention to the issue of racism to a climax. As more people pay attention to this issue, more protests should happen.
- Reflection 3: Does the change in the number of protests from 2018 to 2019 to 2020 surprise you? Why or why not? What do you think explains the fluctuation? Please answer in 1 or 2 sentences (2 points)
What surprised me is that there were more protests in 2018 than in 2019. I think the explanation should be that fewer protests on the issue of racism in 2019 make it more serious in 2020.

- Reflection 4: What is the first and fourth most frequent category of protest? Do these frequencies align with your sense of the major protest movements in the U.S. in the last few years? Why or why not? (3 points)
Racial Injustice is the first most frequent category of protest and Immigration is the fourth most frequent category of protest. These frequencies align with my sense because more immigration happen in recent years and Immigrants are a particularly vulnerable group.
## After You Code: Critical Analysis & Reflection

In the second chapter of *Data Feminism*, Klein and D'Ignazio describe 4 ways that data scientists can challenge power and take action:
> Taking action can itself take many forms, and in this chapter we offer four starting points:  
> (1) Collect: Compiling counterdata—in the face of missing data or institutional neglect—offers a powerful starting point as we see in the example of the DGEI, or in María Salguero’s femicide maps discussed in chapter 1.  
> (2) Analyze: Challenging power often requires demonstrating inequitable outcomes across groups, and new computational methods are being developed to audit opaque algorithms and hold institutions accountable.  
> (3) Imagine: We cannot only focus on inequitable outcomes, because then we will never get to the root cause of injustice. In order to truly dismantle power, we have to imagine our end point not as “fairness,” but as co-liberation.  
> (4) Teach: The identities of data scientists matter, so how might we engage and empower newcomers to the field in order to shift the demographics and cultivate the next generation of data feminists?  

- How does the CountLove project embody one or more of these 4 forms of challenging power? Please answer in at least 3-4 sentences (3 points)
 I believe CountLove project embody the first and forth forms of challeenging power.  Tommy Leung and Nathan Perkins worked on our Masters in Technology and Policy in MIT which demonstrate their strong background about this topic. Also, even the records of protests from newspaper didn't mention the attendees, they will sate the event.
- What is the most interesting or surprising thing you learned from this analysis? Please answer in at least 2-3 sentences (2 points)
This analysis claim the importance of how to deal with missing data. When I do my research before, I would just ignore the missing data. But now I realize I have to deal with the missing data carefully to make my result more convincing.

- What is a kind of analysis that you would like to do or that would be interesting to do with the CountLove data that you don't have the time or skills to accomplish at this moment? Please answer in at least 2-3 sentences (2 points)
I wonder the number of people who protest for certain reason. For example, how many people protest for healthcare. By knowing this, I can figure out the most serious problem existed now.
