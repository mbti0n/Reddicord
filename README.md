# Reddicord
Parse the newest post in a subreddit and send to Discord using Webhooks

---
## How to use
- To get the information of the newest post in a subreddit (e.g. LGR):
``` python
import Reddicord
getSubreddit = Reddicord.GetReddit("LGR")
```
- To print a dictionary of the information of that post, including the value of title, link, author, date, content, and thumbnail URL:
``` python
import Reddicord
getSubreddit = Reddicord.GetReddit("LGR")
printInfo = test.subredditInfo()
print(printInfo)
```
Output (as of 6:27 PM (EDT), August 5, 2023):
```
{'title': ['Mad Catz steering wheels and pedals'], 'link': ['https://www.reddit.com/r/LGR/comments/15izia2/mad_catz_steering_wheels_and_pedals/'], 'author': ['u/vrphotosguy55'], 'date': ['4:06 PM, August 5, 2023 (UTC)'], 'content': [''], 'thumbUrl': ['https://preview.redd.it/kz1d4ws5fbgb1.jpg?width=640&crop=smart&auto=webp&s=bdd8f6d19036f7389d186f20b607a78d4c978756']}
```
- Execute a Discord Webhook of that post:
``` python
import Reddicord

getSubreddit = Reddicord.GetReddit("LGR")
getSubreddit.execute(<your_Webhook_URL>)
```
Output:

<img width="374" alt="image" src="https://github.com/mbti0n/Reddicord/assets/105599214/20b46df7-7eb0-45a1-9ea6-ad57b63ce416">
