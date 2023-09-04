## Investigating the COVID-19 vaccine discussions on Twitter through a multilayer network-based approach 
By Gianluca Bonifazi, Bernardo Breve, Stefano Cirillo, Enrico Corradini, Luca Virgili
[ [Paper](https://www.sciencedirect.com/science/article/pii/S0306457322001960) ]

### Abstract
Modeling discussions on social networks is a challenging task, especially if we consider sensitive topics, such as politics or healthcare. However, the knowledge hidden in these debates helps to investigate trends and opinions and to identify the cohesion of users when they deal with a specific topic. To this end, we propose a general multilayer network approach to investigate discussions on a social network. In order to prove the validity of our model, we apply it on a Twitter dataset containing tweets concerning opinions on COVID-19 vaccines. We extract a set of relevant hashtags (i.e., gold-standard hashtags) for each line of thought (i.e., pro-vaxxer, neutral, and anti-vaxxer). Then, thanks to our multilayer network model, we figure out that the anti-vaxxers tend to have ego networks denser (+14.39%) and more cohesive (+64.2%) than the ones of pro-vaxxer, which leads to a higher number of interactions among anti-vaxxers than pro-vaxxers (+393.89%). Finally, we report a comparison between our approach and one based on single networks analysis. We prove the effectiveness of our model to extract influencers having ego networks with more nodes (+40.46%), edges (+39.36%), and interactions with their neighbors (+28.56%) with respect to the other approach. As a result, these influential users are much more important to analyze and can provide more valuable information.

### Install dependencies
`pip install -r requirements`

### Dataset
Add in the dataset folder the tweets to analyze. Three files are required:
- **verified_tweets**: .json file containing the list of tweets.
- **verified_users**: .csv file containing the username and user id of verified users.
- **likes**: .csv file containing the the tweet id, the user id that liked that tweet, the user id that made that tweet, the corresponding usernames and the tweet text.

### Network
In the network folder, the reply and retweet graphs will be generated. In the next days, we will upload the generation of mention and like graphs.

### Notebook
- **Create-Networks**: create the reply, mention, like and retweet networks.
- **Network-Analysis**: analyze the previously created networks as a single network and as a multilayer network.