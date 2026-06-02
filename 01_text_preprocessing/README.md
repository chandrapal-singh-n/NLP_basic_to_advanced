Text pre-processing (these are the tasks to be done)

-> Lowercasing: it is a process to convert all uppercase characters into lowercase to standardize text data. Have to be cautious in NER case i.e.
"General Motors" to "general motors", acronyms ie "US" to "us" etc.

-> HTML Tag Removal

it removes all HTML tags and retain the text 
it uses regex to match (import re which allows to match and replace text pattern)

re.compile (<.*?>)
match any character =.
match zero or more occurences = *
match non-gredy = ?

-> URL Removal

re.compile(r'https?://\S+|www\.\S+')
r = raw string
https:?= match http or https as ? previous charcater s is option so it matches both http and https both 

://  to match :// in link

\S is used for matching any non-white but doesnt match tab, whilespace , new line therefor e
S+  means one or more  matches everything until a space occurs.



|  A or B


http://...
https://...
or 
www

-> Punctuation Removal

-> Chat word 

-> Spelling correction

-> Stopword removal

-> Handling Emojis

-> Tokenization 

-> Stemming

-> Lemmatization 

Stemming, lemmatization are the text normalization methods which are used to ensure that the words are represented in their base form  