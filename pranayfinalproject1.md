# Telling Stories with Data - Part I: Final Project - Pranay Raj (pranayrp)

# High Level Summary
In 2023, Netflix for the time in years released something that none of the streaming companies have since the beginning of streaming: Data. Off the demands of the writers' and actors' strike, streaming platforms have increasingly become aware they need to release data. Netflix released a list of all watched titles (18000+) with their streaming minutes from the months of January-June 2023.

<img width="888" alt="image" src="https://github.com/pranayrp/portfolio/assets/157341264/e6ce737e-bdb0-4b7a-9254-a6a0d0861bfe">

However, the data feels unorganized - consistency isn't maintained with naming titles, no way to understand if a title is a series or not if the word 'Season' isn't present. I personally felt Netflix dumped data out of obligation and they dumped it in a such a way, I believe they felt viewers wouldn't be interested in the data if it were presented/released this way.


My audience for this project are companies performing entertainment analytics and my intention is to show Netflix's data can actually be very informative if coupled with the right kind of data. The data I shall be combining are:
1. Rotten Tomatoes Rating: The rating of each title will help one understand if the popularity of a show in today's world relies on critics rating or not. <br /> 
2. Netflix Original (Y/N): This will help understand how reliant Netflix is on licensed shows than their Originals.
3. Runtime: This will help understand if audiences (who are part of an era where short form content is thriving) are making decisions on what to watch based on runtime of the movie or length of series. <br /> To interpret this data better and make more specific conclusions, I shall also be coupling data such as the genre and format of each film/series. <br /> 

# The Story
As I start off with my visualization, I'll begin talking about how Netflix released data earlier this 2023, something none of the streaming companies have every done before. I shall go into probably why they didn't do it before and why they have to now, considering the terms and results of the writers' and actor's strike, and certain US policies. Following that, I shall show them the data that Netflix released and how it seems unorganized and uninformative - as if they don't want the viewer to even scroll or pay much attention to it. <br/> 

I shall dive into how, for the sake of the presentation, I've picked the top 500 titles to better explain how informative this data can be. I'll display the way I've revisualized Netflix data for the top 500 titles. I shall even show a world map of where all the titles are from. <br/> 

I shall then move on to explain the data I'll be combining with these titles- (1)Rotten Tomatoes Ratings (2)Netflix Original (Yes/No) (3)Runtime. I shall also be segmenting data into further columns like Movie/Tv Series and Genre to better understand motivations of viewers. In the end, I shall tell how inorder to analyze neutral unskewed data, I have only picked titles that are Globally available. 

**Rotten Tomatoes Rating**:- <br /> 
Setup: Do critics ratings impact viewership? I shall show audience the ratings for the top 500 titles in the Neflix data<br /> 
Conflict: I would then begin showing observations - how the most watched show on Netflix 'The Night Agent' has only 74% while other shows have much lower rating. I shall also talk about certain outlier titles that have extremely low ratings yet have caught massive attention of viewers. <br /> 
Resolution: I shall define a good show to be one that has above 80% rotten tomatoes rating and therefore, I'm likely to conclude that ratings do possibly push a viewer to watch a show.

**Netflix Original(Y/N)**:- <br /> 
Setup: During the pandemic, Netflix struggled to produce content due to quarantine laws. At this junction, the business depended heavily on licensing existing movies and tv series on the platform. Following a spike in viewership for this, the platform is said to have gradually moved towards licensing more movies and shows post-pandemic too. The reborn fandom for series like 'Manifest' and 'Suits' last year is a testament to what licensing has achieved for Netflix. The aim is to deduce how many of the titles seen in 2023 are Netflix Originals or not. <br/> 
Confliect: I would dive into how most of the top shows are Netflix Originals. However, among the 1000, majority are licensed shows. I would then dive into how it's impossible to produce a 1000 shows in a year and therefore licensing is inevitable. At this junction, I will then take a random sample of 10 movies and 10 series in the list and focus on whether the sum of viewing minutes is greater for Originals or for licensed in each of these samples. <br/> 
Conclusion: Netflix's plan of licensing content should continue considering the current interests in licensed shows. <br/> 

**Runtime**:- <br/> 
Setup: In the last decade, due to the rise of short form content, audience's attention span has decreased. As a result, not only do they expect a lot more in the short time they spend of content, they also are not willing to allocate too much time to a particular content. The aim is to notice any particular patterns in the runtime for movies/no. of episodes of each series. <br/> 
Conflict: While we do notice a trend where movies with shorter runtime and limited series were viewed more, we also notice many movies and series with much longer runtime/episodes having immense viewership. For these particular titles, I dissected them into the genres they belong to to understand if there is a pattern to  be understood here. <br/> 
Conclusion: Titles with huge viewership in the Netflix were noticed to have either shorter runtimes or came under a particular genre that seems to be the taste of most audience. <br/> 

As I end my presentation, I shall show a final picture of all the charts I've displayed so far to conclude how valuable and informative Netflix's titles can be and ask them to look out for the data of Aug-Dec 2023

As I conclude my presentation, I shall show my audience one last look at the array of charts I've presented, reminding them the wealth of valuable and informative insights Netflix's data can give us. I'll then encourage them to keep an eye out for the upcoming data from August to December 2023!

# Initial Sketches and Code

![Adobe Scan 13 Feb 2024_1 (1)](https://github.com/pranayrp/portfolio/assets/157341264/7fef0fdd-f5b6-468c-814d-d776eeaf9227)

<img width="646" alt="Code 1" src="https://github.com/pranayrp/portfolio/assets/157341264/6264ce9c-9264-4bf6-b771-be5390b437c8">

<img width="625" alt="image" src="https://github.com/pranayrp/portfolio/assets/157341264/478a80a8-e61c-4205-8d2e-a211a638bc5c">

<img width="590" alt="image" src="https://github.com/pranayrp/portfolio/assets/157341264/5851505a-8b2f-4b4d-bf12-6766f739cbd9">


# The Data
All above data is pubicly accessible. The herculian task is to bring data for each of these titles from seperate sources. Netflix's report can be found here: https://assets.ctfassets.net/4cd45et68cgf/1HyknFM84ISQpeua6TjM7A/97a0a393098937a8f29c9d29c48dbfa8/What_We_Watched_A_Netflix_Engagement_Report_2023Jan-Jun.xlsx </br>
As seen, the report includes:  Title, Viewing Minutes, and Global availablily.<br/> 

For the  Rotten Tomatoes Rating, I have written a python script that scrapes google homepages. Everytime someone googles a title, information regarding the title's rotten tomatoes review and rating shows up. The python tool I've build will input all data pertaining to Rotten Tomatoes into an Excel. In this Excel, I've written a formula to erase all unnecessary data, such that each cell only contians the RT rating.<br/> 

For Netflix Originals or not, I first researched if all 'Globally available' titles are Netflix Originals or not. I was informed sometimes Netflix Originals aren't globally available due to distribution and censorship hinderances. Following which, I copy-pasted all Netflix Originals data from the Netflix wikipedia page. I copied the titles into an excel. I then wrote a python script that verifies if the titles in the released data are present in this excel. Following which, I mapped the data and created a Netflix Originals (Y/N) column. For anomalies that weren't detected, I manually googled the data for each title. For Runtime, I've used an pre-existing OMDb API that logged in every title's runtime.<br/> 

# Method and Medium

I plan on using Tableau for my Final Project. I intend to create a dashboard for each area of data I'm diving into to take audience through a story/journey. I shall begin with a glimpse of the data Netflix released, then show my visualization of that data, a world map of where titles are from and then dive into the areas I've specified above.

