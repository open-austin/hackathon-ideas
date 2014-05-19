# Collect and Graph City Lobbyist Data

Submitted by: [Matt Carey](https://github.com/mscarey)

_If you want to support this proposal, add your feedback [here](https://github.com/open-austin/hackathon-ideas/issues/12)_

### Who will benefit the most from this project?

Muckrakers.


### What is the problem you are trying to solve by participating in the hackathon?

The dates of registration/renewal aren't included in [the lobbyist dataset on Austin's data portal](https://data.austintexas.gov/dataset/Lobbyists/bqav-9x6a) and they have to be inferred based on the dates of expiration included in the dataset. The categories in the “Nature of Business” field aren't very standardized. It's very hard to tell when a company or industry hired lobbyists.


### What evidence (anecdotal or otherwise) do you have that this is a need?

The "Nature of Business" field for Uber in the lobbyist database shows "Information Technology" while the same field shows "Transportation" for Lyft and "Taxicab" for Yellow Cab. Graphing these categories in Socrata wouldn't reveal any useful trend. The fact that Yellow Cab is higher up in the dataset suggests it's been lobbying longer, but we don't know how much longer. I suspect the city occasionally changes the existing fields in the dataset and deletes the old expiration dates, which means valuable information will no longer be available to the public unless we archive it.


### What resources will you be providing to support the development team?

Some links? We could try to standardize the corporation names in the dataset and tag them with unique identifiers to connect them to the corresponding page on OpenCorporates.

https://api.opencorporates.com/documentation/Google-Refine-Reconciliation-API

> The Google Refine Reconciliation API allows Google Refine users to match company names to legal corporate entities. 

https://api.opencorporates.com/documentation/REST-API-introduction

> The OpenCorporates REST API is a simple but powerful API for retrieving information from the OpenCorporates database.  

[OpenCalais](http://www.opencalais.com/about) is an alternate tool that might be able to identify corporations by their names, similar to Google Refine.

And we could look into using the [“Global Legal Entity Identifier System”](http://openleis.com/info/about_the_LEI_system). 


### List current solutions and why you need a new approach to be developed:

Aside from the Socrata database, there's [a search form](http://www.austintexas.gov/cityclerk/lobbyist/index.cfm) on the city website. It's not easy to find anything unless you know exactly what you're looking for, and it's not easy to visualize trends over time.


### At the end of the weekend, what does success look like? What are your expected outcomes?

There are a few possibilites.

1. We simply ask the city to supply a separate dated line in the dataset for every registration or renewal, and they say yes. (Or they even add [all the data that Chicago provides](https://data.cityofchicago.org/Ethics/Lobbyist-Data-Lobbyist-Registry-2012-to-present/ypez-j3yg))
2. If the dataset doesn't improve, we periodically make our own archive of the dataset so the old expiration dates don't get lost. Then, assuming the registration/renewal dates are exactly one year before the expiration dates, we'll know when clients are hiring or renewing lobbyists.
3. We create an interactive timeline to visualize the dataset to show how many lobbyists there were on any given date, broken down by client and by industry. It would be good if we could use the same [standard industry categories used on followthemoney.org](http://www.followthemoney.org/database/IndustryTotals.phtml).
4. An ambitious extra goal would be to create a timeline of press coverage of the word “Austin” and the client's name, alongside the timeline showing how many city lobbyists the client had at any given time. Neither the Texas Tribune nor the Statesman seems to have an API for this, but [the New York times has one](http://developer.nytimes.com/docs/read/article_search_api_v2), and other news outlets might have them too. (See [Feedzilla](https://code.google.com/p/feedzilla-api/wiki/RestApi))




