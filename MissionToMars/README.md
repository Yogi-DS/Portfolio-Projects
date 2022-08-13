##  Mission2Mars
It is a webapp which has interesting facts about planet Mars, weather of Mars, News and pictures of Mars. App involves web-scraping using BeautifulSoup, Flask, PyMongo. It scrapes the news details and images from NASA websites.
For news and information, app uses this web address: ["https://mars.nasa.gov/news/"](https://mars.nasa.gov/news/).
For Images, it uses: ["https://www.jpl.nasa.gov/spaceimages/?search=&category=Mars"](https://www.jpl.nasa.gov/spaceimages/?search=&category=Mars)

### Example outputs
''' 
# Use the parent element to find the paragraph text
news_p = slide_elem.find('div', class_="article_teaser_body").get_text()
news_p
'NASA’s next mission to Mars, InSight, is scheduled to launch Saturday, May 5, on a first-ever mission to study the heart of the Red Planet.'
'''


### Examle Image output
![Mars Image](https://github.com/Yogi-DS/Portfolio-Projects/blob/main/MissionToMars/images/full.jpeg)


![Mars Facts](https://github.com/Yogi-DS/Portfolio-Projects/blob/main/MissionToMars/images/mars-facts.png)
