# IndianMediaNegativity
A project to assist readers with choosing their online media house of choice and performing further analysis.
The reason why I did this project is [here]()
Check out the end product [here](https://datastudio.google.com/reporting/319d07ad-3499-46ab-b140-4cdfd7df55b4)

<img src="https://github.com/swahareddy/IndianMediaNegativity/blob/master/Readme%20images/firsttable.png" >

## How to run
* Create a BigQuery database with schema from `asda`
* Install python dependancies in requirements.txt
* Add/remove source websites from the `dsfsd`

## Pipeline logic for this project
1. Get news article info from [newsapi.org](https://)
<img src="https://github.com/swahareddy/IndianMediaNegativity/blob/master/Readme%20images/organisations.png">

3. Follow the link to actual article and scrape content

4. Use GCP Nat Lang  API to get sentiment from this scraped content

5. Use GCP to asssign category to the article

6. Write to DB
<img src="https://github.com/swahareddy/IndianMediaNegativity/blob/master/Readme%20images/psotiive.png">
<img src="https://github.com/swahareddy/IndianMediaNegativity/blob/master/Readme%20images/negative.png">

7. Visualise from DB (using data studio)

