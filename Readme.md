I only have two weeks before the new job so lets do some stuff!
## What am I doing with this repository? 
Eventually this will be a platform. Set up as a github organization.
Displaying code examples.
Automating nitty gritty. Using the simplest languages and frameworks to showcase specific useful things you can do at Runtime. This will not be one language but different languages that work best for each example..

## What it is now and what it also will be:
Currently I will be putting things in here as I discover them. Simular to this repository I created for github commands: https://github.com/mapFactory/Github_Map_Closing_Notes

## Here Goes!
Runtime relates to program execution time. Whenever you want to make something scale RAM and Runtime is where that often happens! Common practice is to persist state in the Database or any other filetype. Moving out of RAM persisting to a Database changes the hardware; you are putting information into secondary storage. Accessing that information later will cause latency every time you reach into secondary storage to page it into RAM. Often you do not want to touch a database because it is slow. But if you do. Try to get everything all at once! Every time you touch the database or file will cost you. You will experience Latency and then time required to page in. However, get information from the database and make another request to the database you are stacking latencies. That would be sloooow! Or if you did it all on the same thread and did not paralellize, again stacking latencies, slooooow!

Usually you wont run into this problem but you have 8gb of ram. Your program rarely will take up 8gb of ram. However, if you go over your limit. The program will perform throttling, paging items stored but not accessed frequently in ram to secondary storage. And upon request paging them back into RAM. Oh no! That happens sometimes with video games. Very Slow!! So try to load as much as you can from the database when you can. But dont consume more than your ram can comprehend!
