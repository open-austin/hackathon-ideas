# Pet Finder

Submitted by: [Chip Rosenthal](https://github.com/chip-rosenthal)

*If you want to support this proposal, add your feedback [here](https://github.com/open-austin/hackathon-ideas/issues/3).*


### Who will benefit the most from this project?

All the very sad cats and dogs who have lost their people.


### What is the problem you are trying to solve by participating in the hackathon?

A missing pet is one of the most distressing experiences a person may have. We want to help with that.

From the city perspective, every stray animal takes a sorely needed space in our overcrowded shelters.

The sooner we can get the animal back home, the more space we have available for animals in need.


### What evidence (anecdotal or otherwise) do you have that this is a need?

http://austin.craigslist.org/search/pet?zoomToPosting=&catAbb=pet&query=lost&excats=


### What resources will you be providing to support the development team?

Pet intakes are currently posted on the data.austintexas.gov data portal, but those postings occur after the fact,
and are not useful for providing current lost/recovered pet status.

The city animal shelter does push lost pet notices in real time to this website:

http://www.petharbor.com/

We propose setting up a process to scrape the set for local recovered pet information, and use that as the basis for a notification app.

### List current solutions and why you need a new approach to be developed:

Current solutions are:
* neighborhood email lists
* wider bulletin boards and sites, such as Craig's List
* the aforementioned Pet Harbor site

The Pet Harbor site, unfortunately, is not an easy site to use, and does not offer notification support.

The city presents a search of the Pet Harbor site here: http://austintexas.gov/page/view-all-pets

### At the end of the weekend, what does success look like? What are your expected outcomes?

A tool that periodically scrapes pet recovery postings and saves them to a database.
An open API that allows the public direct (machine readable access) to the lost pet data.
A web tool that allows easy search of current lost pet data.
The ability to place an alert when a new lost pet is recovered.
