# High level summary: 
In 2023, Netflix for the time in years released something that noone hasn't since the beginning of streaming: data. Off the demands of the writers' and actors' strike, streaming platforms have increasingly become aware they need to release data. Netflix released a list of all watched titles (18000+) with their streaming minutes from the months of January-June 2023. While Netflix did release data, I personally felt they dumped it out of obligation. The data is not filtered or descriptive of anything. However, given the right kind of data to go with it, one can actually deduce a lot from this data. For my final project, I've decided to adjoin data to Netflix's data to make certain deductions. The data I shall be combining are:
1. Rotten Tomatoes Rating: The rating of each title will help one understand if the popularity of a show in today's world relies on critics rating or not
2. Netflix Original (Y/N): During and post-pandemic, Netflix has relied increasing more on licensing than producing a show. The aim is to figure how many of these titles are Netlflix Originals and how many aren't
3. Release Data: There's been a growing trend lately of old shows being discovered. For example, Suits. Seeing how many top-viewed shows were actually old and then adjoining their genre, could speak a lot about the audience.

Method and Medium:
All above data is pubicly accessible. The herculian task is to bring data for each of these titles from seperate sources. 
The report released by Netflix includes:  Title, Viewing Minutes, and Global availablily.
For the  Rotten Tomatoes Rating, I have written a python script and scrapes google homepages. Everytime someone googles a title, information regarding the title's rotten tomatoes review and rating shows up. The python tool I've build will input all data pertaining to Rotten Tomatoes into an Excel. In this Excel, I've written a formula to erase all unnecessary data, such that each cell only contians the RT rating.
For Netflix Original or not, I first researched if all 'Globally available' titles are Netflix Originals or not. I was informed sometimes Netflix Originals aren't globally available due to distribution and censorship hinderances.
For Release Date, I've used an pre-existing OMDb API that logged in every title's release data.
