# ppr_project
Examining whether PPR scoring methods fairly balance WR scoring to RB, or if it unfairly overvalues players who record many receptions.

**Background**
Fantasy football works by drafting teams, like portfolios of players. These players' game performances are translated into fantasy points mostly on yards gained and points scored.
Somehwere along the line, fantasy managers thought that RBs usually get more yards while scoring similar numbers of touchdowns. 
So some league managers decided to balance this difference in positions by awarding a full point for each time a player catches a ball, regardless of the yards gained.
This drastically changed the draft strategy, placing more emphasis on WRs _and_ RBs who catch more passes. 

In one of my leagues, we tried full ppr for a year, but found that it altered typical fantasy strategy too much. 
It is also frustrating to lose close games against players who catch many balls for low yardage.
Thus, we agreed to compromise by moving to half ppr, which means each reception earns .5 points.
This is a happy medium for us, but another of my leagues operates under full ppr and is not open to change.

This analysis is a personal, and maybe evidenciary, excersise in testing a hypothesis:
Again, that full ppr overvalues pass-catching players. 

**Method**

I started with the player stats for the 2019 season, unable to find free access to more recent data.
From there, I added columns for their fantasy points season total with standard scoring, .5 ppr, and full ppr.

I made 100 random teams with 2 RBs, 2 WRs, and 1 TE. I was considering dividing them into leagues, but determined that would be an unecessary step in generating random team scores.
I also considered adding some draft logic (maybe based on ADP, which predicts where the player will be drafted) but determined that would be again unecessary. 
Fantasy players will know that random darft logic isn't far off from most players' drafting strategy.

Now, how to determine if full ppr is unfair.

I did a visualization that showed the top 50 players at WR and RB, graphing their scores under standard, half ppr, and full ppr. 
This shows that it boosted WRs overall, and boosted few RBs signifcantly.

So, I thought that standard deviation would be a good measure to see whether team scores are more variable under ppr rules than not. This returned very large standard deviations, 
so I will need to rethink my analysis here.

Part of the reason scoring methods are significant is that they change draft strategy. Maybe a simple analysis would be to see how teams with 2 RBs and 3 WRs compete against teams 
with 3 RBs and 2 WRs. And this would track with real world drafting, as teams draft a Flex as well, who can be WR or RB. 
This way, we can compare teams that emphasize WRs over RBs and vice versa, without introducing draft logic. 



