# The potential for high-speed sleeper trains in Europe

## Introduction

The expansion of high speed rail in many regions of the world has really transformed medium-distance travel. In particular, Europe has seen huge expansions of the network, from the original LGV network in France to coverage across Germany, Spain, Belgium, the Netherlands and elsewhere. Globally, this development has been significant too: the Chinese market is significant, Japan has long since had a good high speed rail network. Even the USA is now getting on with some things!

Across many city pairs, such as London-Paris and London-Brussels (covered by Eurostar), high speed rail has taken significant market share from airlines `need stat`. On short journeys (in the hundreds of kilometers), high-speed rail is very competitive on time once you take into account the time taken to travel from city centres to airports on either end and the time taken to pass through security checks.

Despite concerns about a decline in operation, sleeper train services are also gaining popularity with the rise of the *flygskam* phenomenon - ÖBB’s railjet service, the backbone of the sleeper train services across Europe, has recently announced expansion `need stat`. However, mthe vast majority of rail sleeper services operate at significantly lower speeds than their daytime counterparts - for instance, `need further explanation here`. Most of the stleeper train stock across Europe is older than the high-speed stock, and is not capable of operating at true high speed.

However, there is an opportunity to combine the high-speed rail and sleeper train concepts. Reducing the journey times on a sleeper train by an hour or two would not normally be considered as large a benefit as the same time reduction on a daytime service, but the real benefit of these services would be in operning up new routes which are not already served by sleeper trains because the journey is considered to be too long. For instance, the longest duration of sleeper train service operated by ÖBB Nightjet is the Zagreb-Zürich sleeper, which departs Zagreb at 18:38 and arrives in Zurich the following morning at 09:20 the following morning, a duration of 14 hours 42 minutes. Many sleeper services have much shorter durations, allowing for a late evening departure and an arrival in time for a morning meeting or a full day of sightseeing. So, high-speed sleeper trains could allow much longer routes to be covered in a reasonable night-time journey.

There are a few reasons why high-speed sleeper operations could be quite attractive. Firstly, most of the infrastructure required is already in place. In contrast to schemes for the development of new rail lines, the investment in heavy infrastructure is minimised. Secondly, a lot of high-speed rail inrfastucture is modern, built to high standards and in very good condition. As a result, night-time closures for maintenance are not as commonplace (HS1 in the UK, for instance, operates a 30 minute closure during the day but otherwise delivers a 24 hour operation). Thus, high-speed sleeper trains offer the opportunity to maximise the use of an existing asset.

## Analysis

Based on this idea, I decided to take a look at some of the data in an attempt to answer the question:

"On which city pairs (if any) across Europe is there a potential for a viable high-speed sleeper train service?"

In order to answer this question, I needed information on (1) current passenger numbers between city pairs (which I got from Eurostat `link`), and (2) information on existing high-speed journey times between those city pairs (which I got from the Hafas API, which powers, among other sites, Deutsche Bahn’s brilliant journey planner). The full Jupyter notebook is available here `link` for reference.

Results, part 1: let’s take a look at travel time vs. passenger numbers

The first observation is that there are many routes across Europe where there are still high air passenger numbers despite a relatively short travel time on rail (in most cases high-speed rail). This is an interesting observation and while the data is not completely up to date there is probably a potential for more modal shift from air to rail along these corridors (leaving aside the sleeper issue entirely).

Filtering down to those journeys with duration 8-12 hours, some corridors do stand out:

However, some corridors do stand out, e.g.:
Barcelona-Amsterdam
Barcelona-London

This could work with an extension to Madrid as well, along the Barcelona-Madrid high speed corridor, e.g. Madrid-Barcelona-Lille-Brussels-Amsterdam (all Schengen, security checks in Madrid and Barcelona) or Madrid-Barcelona-London (needs new passport controls in Spain).

- Look at most popular air corridors in Europe (need volume to extract)
- Compare rail journey time on these corridors
- Some analysis of operational factors
- Any costs
