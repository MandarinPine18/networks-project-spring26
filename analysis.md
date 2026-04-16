# Analysis

1. Which city has the highest inefficiency ratio? Look it up on [submarinecablemap.com](https://submarinecablemap.com) — what cables serve it and how does that explain your result?

Sendai had the highest inefficiency ratio, for my run, with a ratio of 16.53. Sendai is in Japan. This is interestingly despite being geographically close to Tokyo, which had a much lower inefficiency ratio. Looking at the submarine cables, a small part of the delay is the geographic diversion slightly north in the Pacific Ocean, but I think this might have more to do with processing or queueing delays. It looks like Japan might be a point where a lot of trans-Pacific traffic must cross - I'd assume the infrastructure in Tokyo is better-equipped than in Sendai. It also could be possible that congestion on the direct line was so bad that a far less direct route needed to be taken.

2. Which city is closest to the theoretical minimum? What does that tell you about routing infrastructure there?

Seoul had an inefficiency ratio of 1.06, which is very low. The routing infrastructure there and back must be exceptional to support that - the difference between the physical limit and realistic RTT is only around 7ms.

3. Your packet to Lagos almost certainly routes through Europe first. Why does Africa route through Europe, and what would need to change to fix it?

There are very few trans-Atlantic submarine lines from Africa. There are none that run from North America to Africa. Most of African traffic has the shortest physical distance to the USA via European submarine lines. Fixing this would require laying more submarine lines across the Atlantic Ocean to Africa, specifically to North America in our case.
