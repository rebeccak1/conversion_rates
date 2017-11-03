# Conversion Rate
## Goal

Optimizing conversion rate is likely the most common work of a data scientist, and rightfully so.
The data revolution has a lot to do with the fact that now we are able to collect all sorts of data
about people who buy something on our site as well as people who don't. This gives us a
tremendous opportunity to understand what's working well (and potentially scale it even further)
and what's not working well (and fix it).

The goal of this challenge is to build a model that predicts conversion rate and, based on the
model, come up with ideas to improve revenue.

This challenge is significantly easier than all others in this collection. There are no dates, no
tables to join, no feature engineering required, and the problem is really straightforward.


## Challenge Description
We have data about users who hit our site: whether they converted or not as well as some of
their characteristics such as their country, the marketing channel, their age, whether they are
repeat users and the number of pages visited during that session (as a proxy for site
activity/time spent on site).

Your project is to:
- Predict conversion rate
- Come up with recommendations for the product team and the marketing team to improve conversion rate

## Data
The table is `conversion_data`. It has information about signed-in users during one session. Each row is a user session.

### Columns:
- country : user country based on the IP address
- age : user age. Self-reported at sign-in step
- new_user : whether the user created the account during this session or had already an account 
and simply came back to the site
- source : marketing channel source
- Ads: came to the site by clicking on an advertisement
- Seo: came to the site by clicking on search results
- Direct: came to the site by directly typing the URL on the browser
- total_pages_visited: number of total pages visited during the session. This is a proxy for
time spent on site and engagement during the session.
- converted: this is our label. 1 means they converted within the session, 0 means they left
without buying anything. The company goal is to increase conversion rate: # conversions
/ total sessions.
