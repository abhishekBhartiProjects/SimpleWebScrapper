# SimpleWebScrapper
Scrap title of any website through a simple python code

## Library used
- [bs4 - BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
- requests
- lxml

## Code
import requests

import bs4

response = requests.get('https://www.amazon.in/')

formatedResponse = bs4.BeautifulSoup(response.text, 'lxml')

title = formatedResponse.select('title')

t0 = title[0].getText()

print(t0)

---------output------

Online Shopping site in India: Shop Online for Mobiles, Books, Watches, Shoes and More - Amazon.in

![alt text](https://github.com/abhishekbharti-github/SimpleWebScrapper/blob/master/webScrapper.png)
