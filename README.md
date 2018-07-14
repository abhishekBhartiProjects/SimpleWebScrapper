# SimpleWebScrapper
Scrap title of any website through a simple python code

## Code
> import requests

> import bs4

> response = requests.get('https://www.amazon.in/')

> formatedResponse = bs4.BeautifulSoup(response.text, 'lxml')

> title = formatedResponse.select('title')

> t0 = title[0].getText()

> print(t0)

Online Shopping site in India: Shop Online for Mobiles, Books, Watches, Shoes and More - Amazon.in

>>> 
