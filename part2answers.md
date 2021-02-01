Question 1: Hello,

I'm new to search engines, and there are a lot of concepts I'm not educated on. To make my onboarding smoother, it'd help if you could provide me with some definitions of the following concepts:

Records
Indexing
I'm also struggling with understanding what types of metrics would be useful to include in the "Custom Ranking."

Cheers, George

Hi George,

Thanks for your email, I’ll do my best to answer for you below.

Records.
An Algolia record is the representation of an item that you would like to be searchable. It includes values for the attributes that describe the item.
For example, we can define 2 different products called “Umbrella”, one with a colour of red and one with a colour of blue. Each of these is a different record.

Records and their attributes are covered in our documentation here: https://www.algolia.com/doc/guides/sending-and-managing-data/prepare-your-data/

Indexing.
Indexing is the operation that creates searchable results from the individual records described above. Think of an index as a group of search results, and you can create multiple indices from a set of records. 
For example, you may create a price ascending index and price descending index to allow customers to sort by price.

Custom Ranking.
Custom ranking attributes allow you to specify the fields that affect the ordering of search results. Think of these as values that are not searchable but are useful for sorting purposes.
For example, you may add stock level information as a number field, and specify it as a custom ranking attribute, allowing users to sort by items in stock.

Indexing and Custom Ranking have some additional detail here: https://www.algolia.com/doc/guides/getting-started/how-algolia-works/in-depth/implementation-process/

If you would like to discuss further, or if you have any other questions please don’t hesitate to contact me.

Thanks,
Neil



Question 2: Hello,

Sorry to give you the kind of feedback that I know you do not want to hear, but I really hate the new dashboard design. Clearing and deleting indexes are now several clicks away. I am needing to use these features while iterating, so this is inconvenient.

Regards, Matt


Hi Matt,

Thanks for your email, we’re interested in any feedback from our customers so we can see what improvements we can make. I will pass this on to our UI dev team.

In regard to clearing and deleting, there are at least a couple of reasons why these actions are behind a couple of clicks:
These 2 operations are destructive to the data within the indices; in any production environment, clearing or deleting an index will stop search working.
Clearing an index is an expensive operation that would result in request throttling, so should be used with caution.

With destructive operations like these, it is always best to try and minimise their use so as to save server and network time, so the actions are not made available with only one click.

For your iterations, it may be that there are other tools within Algolia that can help you. I’m not sure which features you are iterating, but I would be happy to chat to understand what you are working towards and if there is any other way Algolia can accommodate - while minimising clears and deletes.

If you would like to discuss further, or if you have any other questions please don’t hesitate to contact me.

thanks,
Neil


Question 3: Hi,

I'm looking to integrate Algolia in my website. Will this be a lot of development work for me? What's the high level process look like?

Regards, Leo


Hi Leo,

No it doesn’t have to be a lot of development work - you can install Algolia on your website very quickly and with minimal development effort. For example, you can use the InstantSearch.js library for a “Quickstart” as detailed here: https://www.algolia.com/doc/guides/building-search-ui/getting-started/js/

Actual development choices can be more complex and will depend on your current development environment(s), languages and development experience. Options range from the plugin-like option detailed above all the way to full custom implementation with the language(s) of your choice. Our documentation has a case study implementation that is a good example. https://www.algolia.com/doc/guides/going-to-production/case-study/

We can discuss your current situation and offer some guidance for the best outcome. Let me know if you would like to do this.

thanks,
Neil
