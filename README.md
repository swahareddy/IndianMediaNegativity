# IndianMediaNegativity
A project to assist readers with choosing their online media house of choice and performing further analysis.

### The reason why I did this project is [here](https://medium.com/@swahareddy/if-it-bleeds-it-leads-a4739cee9284?sk=1bd0b0fcfc6cdca266aca86467bbf590)

### Check out the end product [here](https://datastudio.google.com/reporting/319d07ad-3499-46ab-b140-4cdfd7df55b4)

<img src="https://github.com/swahareddy/IndianMediaNegativity/blob/master/Readme%20images/firsttable.png" >

## How to run
1. Create 2 BigQuery tables with schema from [`master_table.schema`](https://github.com/swahareddy/IndianMediaNegativity/blob/master/master_table.schema)
2. Install python dependancies in [`requirements.txt`](https://github.com/swahareddy/IndianMediaNegativity/blob/master/requirements.txt)
3. Add/remove source websites from the notebook
4. Run the jupyter notebook


- [ ] Create 2 BigQuery tables with schema from [`master_table.schema`](https://github.com/swahareddy/IndianMediaNegativity/blob/master/master_table.schema)
- [ ] Install python dependancies in [`requirements.txt`](https://github.com/swahareddy/IndianMediaNegativity/blob/master/requirements.txt)
- [ ] Add/remove source websites from the notebook
- [ ] Run the jupyter notebook

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


### About databases
The articles and their metadata are 'streamed' (to avoid daily rate limits of BQ) into an interm/staging table. 

The interim table and master table are compared (same schema), and any new additions are pushed into master table. (Needed since same article can come in multiple responses from newsapi.org API) 
_________________
If you have not used GCP before, go through [this](https://github.com/swahareddy/IndianMediaNegativity/blob/master/gcp_guide.md)
