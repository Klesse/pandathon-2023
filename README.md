# 🐼 Pandathon 2023 📊

In this challenge, we had to create a web-scrapping strategy to get data 
about city secretaries from all Brazil🇧🇷..

The only data we had was a csv file with the cities and their anniversaries.

The winner would be the team who had get the most amount of secretaries name, 
i.e., more data, and the team who had create an exploratory data analisys 
with the data.

# First thought

The cities in Brazil has a URL common pattern:

city.state.gov.br

So, with the csv we were able to create a URL for all cities' websites.

# Strategies to get the secretaries names

- with the URLs, we had to stablish a strategy to get the secretaries names.

* Use Spacy to encounter names around the word "secretaria" in pages HTML. ❌
* Gets links in the websites with "secretaria" in it. 🤏
* Combine the two strategies above. ❌
* Use brute force and get data from URL to URL identifying the websites' 
patterns. ✅
* Enter the site with all health secretaries and get the data from there. ✅

### Caption

✅: Done entirely
🤏: Almost done
❌: Not done

# Final strategy

- We focused in getting the health secretaries and, manually, get other 
cities different secretaries. So we finished with more than 5500 row in 
our dataset. We had to find a solution with time limit, so with the health 
secretaries we would have a scope to focus our presentation for the judges 
and our exploratory data analysis on. Training spacy would consume so much 
time, so we discarded this option.

# Used libraries

* Selenium
* BeautifulSoup
* Pandas
* Spacy
* Matplotlib

# Notebooks and their content

- **code1-cities-scrapping**: individual cities scrapper.
- **code2-health-scrapping**: attempts with spacy and the health secretaries 
scrapper.
- **code3-plots**: plots for the exploratory data analysis and the final 
presentation to the judges.

# Authors

Alexandre Gualberto

Ana Carolina Castro Rosal

[Pedro Malandrin Klesse](www.github.com/Klesse)

Vitor Caligaris Figueira
