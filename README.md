# Shark Attack

## Presentation & Objectives <img align="right" src="https://tse4.explicit.bing.net/th?id=OIP.W3zik5hAlXb0d9YLWEjcTAHaDf&pid=Api&P=0&w=346&h=164.jpg" alt="" width="201" height="201" />     

 
#### With this project we intend to create an episode of the TV show Men vs Wild. Is a survival television series hosted by Bear Grylls on the Discovery Channel. The general format of each episode is the premise that Grylls is left stranded in a region with his film crew. The episode documents his efforts to survive and find a way back to civilization, usually requiring an overnight shelter of some kind. There are mostly wild terrains – jungles, forests, or similar non-urban areas.
#### Bear Grylls will simulate a shipwreck in the area where there are the highest number of deadly incidents with the deadliest species in the world. Bear must remain in the animal's habitat until a rescue team arrives at the location.
#### We know that humans are not part of the shark menu, that they often attack out of curiosity or fear. In the following complementary analyzes it is intended to demonstrate what kind of behavior our survivor must have in order not to cause neither curiosity nor fear to one of these incredible animals.

https://www.youtube.com/watch?v=oa6N7agxizw                        



## Status

##### Complete


## Tools used

#### - Pandas library
#### - Regurar expressions
#### - Filters
#### - Grouping


<img align="right" src="https://tse4.mm.bing.net/th?id=OIP.md6AIUrZ7NpkHGMjjio77wHaGB&pid=Api&P=0&w=215&h=176.jpg" alt="" width="201" height="201" /> 

## Development

#### First I removed from the original database the columns to be analyzed: Country, Area, Fatal (Y/N) and Species, I thought it was necessary to rename the Specie column, because it had an unnecessary spacing. I found that many of the lines did not have enough information to do the analysis and the lines that contained more than 20% null values. As the objective is to survive the attack of the deadliest sharks, I selected only the fatal cases. From here I started cleaning the columns separately, starting with Species. This column had a lot of inaccurate information, dirty and even a lot of it didn't correspond to any kind of information of the species. When doing a general reading of the information contained in the column, I found that the vast majority of data that actually contained the species name contained the word "shark" at the end. So I cleaned up by creating a regex from that word. Using the replace method to keep the information clean. After verifying the number of occurrences in each species found, I verified that, in addition to the values ​​cleared by the regex, the values ​​to be cleared are significant in changing the analysis results and I realized that it would not influence the data because the data to be cleared in a sample of 5315 lines would be 1296, and among the 3 deadliest sharks were:

#### - white shark: 619 hits
#### - tiger shark : 254 hits
#### - bull shark: 171 occurrences

#### The rest were below 60 hits.

#### we realize that the "white shark" is the deadliest. Then I did a simple cleaning on the remaining columns, as they weren't too dirty. In the end I grouped the four columns.


# Conclusion

#### With this analysis I found that the father where more deadly attacks of white sharks occur is in the USA, in California, with about 155 occurrences.

<img align="right" src="https://tse4.mm.bing.net/th?id=OIP.OenXsKA8-idaTUbdUVSSFgHaFI&pid=Api&P=0&w=232&h=161.jpg" alt="" width="201" height="201" /> 



# Releases

#### No releases published


# Packages

#### No packages published


# Languages

#### Jupyter Notebook 100%
