# Jigsaw-Unintended-Bias-in-Toxicity-Classification
The Conversation AI team, a research initiative founded by Jigsaw and Google (both part of Alphabet), builds technology to protect voices in conversation. A main area of focus is machine learning models that can identify toxicity in online conversations, where toxicity is defined as anything rude, disrespectful or otherwise likely to make someone leave a discussion. They use data by human raters to improve civility in online conversations for various toxic conversational attributes. 


Data overview
Attribute information:
* comment_text: text of individual comments
* target: toxicity label( to be predicted to for test data. target>=0.5 will be consider to be positive class(toxic))


When the Conversation AI team first built toxicity models, they found that the models incorrectly learned to associate the names of frequently attacked identities with toxicity. Models predicted a high likelihood of toxicity for comments containing those identities (e.g. "gay"), even when those comments were not actually toxic (such as "I am a gay woman"). This happens because training data was pulled from available sources where unfortunately, certain identities are overwhelmingly referred to in offensive ways. 
There are some identity attributes which are taken care:
asian, atheist, bisexual, black, buddhist, christian, female, heterosexual, hindu, homosexual_gay_or_lesbian, intellectual_or_learning_disability, jewish, latino, male, muslim, other_disability, other_gender, other_race_or_ethnicity, other_religion, other_sexual_orientation, physical_disability, psychiatric_or_mental_illness, transgender, white.
