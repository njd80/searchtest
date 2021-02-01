# Notes
  
## Project Outline
I used the Ecommerce dataset. I wanted to use the Movies dataset but I could not get it to load via the dashboard. I think because its more than 50mb.
  
I followed the instructions here: https://www.algolia.com/doc/guides/sending-and-managing-data/send-and-update-your-data/ to add and index the data.
Then I configured the basic relevance settings using https://www.algolia.com/doc/guides/getting-started/how-algolia-works/in-depth/implementation-process/ as a guide.

## Configuration

### Searchable Attributes
  Name, Description, Brand
  
  All are ordered to ensure that relevance is given to each match in order.
  
### Custom Ranking Attributes

  Popularity, Price
  
  To show the most popular and highest price items first to increase conversions and a.o.v.
   
  
### Facets  
I added 'Brand' as a facet so that the filtering widget works.


## What I intended to accomplish
1. Complete the assignment.
2. Make a search interface that was recognisable to me from experience.
  
## Feedback
Getting started does not mention installation of InstantSearch app. So, the first bootstrap command does not work.   
https://www.algolia.com/doc/guides/building-search-ui/getting-started/js/

Even once installed I could not get it to work in that format. Results in the default API key and Index being set.
So - working interface but is using the default API key details. Results look similar so potential for major confusion.

Prerequisites/before you start section on InstantSearch would avoid the confusion.
There are 2 paragraphs that cover instantsearch app installation and module installation, but they are after the "create" command. Move them before and the steps make sense.
