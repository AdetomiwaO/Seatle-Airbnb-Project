# udacity Airbnb Project (Seattle Vibes)

The project is based on the Kaggle dataset:https://www.kaggle.com/airbnb/seattle/data

The resulting blog post can be accessed here: https://medium.com/@adetomiwao/seattle-vibes-ecc152358bb5?source=friends_link&sk=94b6d9f4d47296606682a6210c72e184

The dataset has 3 main files of which I used 2 (listings.csv & reviews.csv)
- calendar.csv: contains listings, availability dates, pricing (4 columns)
- listings.csv: contains detiled information about each listing such as location, url, host comments, average listing scores, neighborhood information and addresses. (96 columns)
- reviews.csv: contains comments from guests about their stay, date of the review, as well as the listing id. (6 columns)

The goal of the project was to tackle a few questions about the data based on NLP and text mining. The questions explored were: 
- Can we identify positive & negative customer reviews ?
- What made the vibe so right (…or wrong) for Seattle Airbnb guests?
- How did neighborhood sentiment change over time?
- What information can we extract from the descriptions of some top neighborhoods?

# Steps Taken:
Reviews: 
- Imported the review data
- checked for missing values
- identified the languages of the reviews
- investigated columns with language that wasn't english 
- created functions to translate foreign languages to english 
- applied gensim preprocessing and calculated sentiment scores using Afinn
- appended listing information to the newly scored dataframe to include location, and housing type. 
- visualized sentiment trends in Power BI

Thanks to the Stack community for tips as well:
https://stackoverflow.com/questions/50910965/how-to-change-seaborn-data-labels-to-show-two-decimal-places

Results suggested majority of sentiment scores from guet reviews were positive. 
Broadway not surprisingly is a top desired neighbourhood but only rose in popularity around 2013.
Host comments were a good indicator for depicting the general vibe of the neighborhoods. Most comments revolved around proximity to major landmarks.


