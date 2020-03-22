---
layout: post
title:      "My CLI Project (Coronavirus Stats)"
date:       2020-03-22 19:12:42 +0000
permalink:  my_cli_project_coronavirus_stats
---


I had trouble deciding what I wanted the subject of my CLI to be. My cohort lead recommended choosing something you’re passionate about, but stuck at home under self-quarantine, all I found myself thinking about was the Coronavirus. So I thought, *“Well, why don’t I just make my project around that?”*, so I did!

I built a CLI that displays up-to-date stats about COVID-19. You can view world totals, active cases, and closed cases. And, you can view stats per country. It scrapes all of its data from the WorldOMeter website.

Here’s the workflow that worked for me:
1. Start with a Scraper class that scraped all needed data from the WorldOMeter website
2. Send that data to respective classes: Virus and Country
3. Virus class represents all world data, and *has many* instances of Country class
4. Country class represents data of a specific country
5. Lastly, a CLI class that initializes the scraper and manages the user interface


I had a lot of fun making this! It was cool to use everything we’ve learned that past few weeks, from Ruby basics to object oriented design patterns. The only hurtle I ran into while making this was choosing how to best delegate responsibility among my classes. Watching Avi’s many lectures on OOP really helped. In the end, I'm really happy with how it turned out.

