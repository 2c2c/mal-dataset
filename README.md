Myanimelist doesn't have a (real) recommendation engine built into its website. It has a lot of user rating data though.

Getting that data can be a challenge. There aren't official APIs to acquire the information. This means that anyone who wants to play with the idea of building a recommendation engine has to find some ad hoc way of scraping together the data. That's bad for MAL's servers and bad for a programmer's time.

I'm publishing this on the off chance it saves someone time.

The format is `userid, animeid, rating, genreid`. Most movie recommendation datasets would have a rating timestamp instead of a genreid, but I didn't have timestamps to scrape.

disclaimer: I scraped the users in this dataset through the MAL clubs section of the site. It's not truly "random".

```
C:\Users\2c\Desktop\mal-ml>python unique_users.py
ratings: 11074405
users: 70421
animes: 13466
```