---
layout: post
title: Vaccinations vs Votes
tags: COVID MathInTheNews PharmaAndBiotech Politics Statistics
comments: true
---

Back in April, we did some [statistical analysis showing Trumpy states tended to have dramatically lower vaccination rates]({{ site.baseurl }}/politics-vs-mask-and-vaccine-use/).  Is that still the case?  Regrettably, yes.  More than ever.  


## Where We Last Left Off in April  

Let's recap our analysis of last April. <sup id="fn1a">[[1]](#fn1)</sup>  

<img src="{{ site.baseurl }}/images/2021-04-19-politics-vs-mask-and-vaccine-use-omnibus.jpg" width="400" height="131" alt="Omnibus dataset: state, voting data, vaccine uptake/usage data" title="Omnibus dataset: state, voting data, vaccine uptake/usage data" style="float: right; margin: 3px 3px 3px 3px; border: 1px solid #000000;"/>
We looked at, among other things, vaccination data from the CDC and the state popular vote
margins for Trump vs Biden.  We assembled all that from a couple disparate sources into an
omnibus dataset. <sup id="fn2a">[[2]](#fn2)</sup>  

<img src="{{ site.baseurl }}/images/2021-04-19-politics-vs-mask-and-vaccine-use-significances.jpg" width="400" height="105" alt="Hypothesis test significances: % doses used, % population vaccinated vs Trump Margin" title="Hypothesis test significances: % doses used, % population vaccinated vs Trump Margin" style="float: right; margin: 3px 3px 3px 3px; border: 1px solid #000000;"/>
<img src="{{ site.baseurl }}/assets/2021-04-19-politics-vs-mask-and-vaccine-use-plot-boxplot.png" width="400" height="600" alt="Discrete: % doses used, % population vaccinated vs Trump Margin" title="Discrete: % doses used, % population vaccinated vs Trump Margin" style="float: right; margin: 3px 3px 3px 3px; border: 1px solid #000000;"/>
<img src="{{ site.baseurl }}/assets/2021-04-19-politics-vs-mask-and-vaccine-use-plot.png" width="400" height="400" alt="Continuous: % doses used, % population vaccinated vs Trump Margin" title="Continuous: % doses used, % population vaccinated vs Trump Margin" style="float: right; margin: 3px 3px 3px 3px; border: 1px solid #000000;"/>
Using that dataset, we did a discrete analysis by $t$-test to see if the mean vaccination
level differed between Trump states and Biden states by popular vote, and a continuous
regression analysis of vaccination percent on the Trump - Biden margin.  Both analyses
came up statistically significant: the Trump states are less vaccinated (1st or 2nd shot),
and this effect is highly unlikely to be due to chance.  The effect size was large enough
to be bothersome, as confirmed by public health officials.  


## A July 4th Meditation on Willful Ignorance on the American Right  

So why revisit this now?  

Basically, Biden promised (actually more like "hoped" and promised to "work real hard")
that 70% of the US population would be vaccinated by the 4th of July so we could all have
barbecues.  That was ambitious, but with the vaccination rates seen in March or April, it
could have been achieved.  

_Could_ have.  

Since then, vaccination rates have leveled off and then steeply declined.  Everybody who
was easy to vaccinate has been vaccinated.  We have a couple of problems:  
- The JnJ vaccine was taken out of use for too long, and people never quite understood the
  thrombosis risk compared to anything else.  We quantified those a 
  bit <sup id="fn3a">[[3]](#fn3)</sup> <sup id="fn4a">[[4]](#fn4)</sup> <sup id="fn5a">[[5]](#fn5)</sup> <sup id="fn6a">[[6]](#fn6)</sup>,
  but this is just a crummy little blog with about 6 readers worldwide (one of whom is my
  cat).  So that didn't help much, other than personally, to soothe my mathematical itch.  
- We've reached everybody who's easy to reach, worldwide. <sup id="fn7a">[[7]](#fn7)</sup>
  Now we have to do _serious_ outreach: in other languages, using local community leaders,
  using local trusted physicians, &hellip; basically using all sorts of outreach to
  communities that are sometimes justifiably suspicious of the US medical establishment.
  We're doing all that, but&hellip;
- Now we're down to hard-core right-wing vaccine resistance, verging on outright refusal
  and deeply irrational rage.  
  
So of all those potential things, is the last one really a driver?  Our state-level
regression analysis in April said yes.  We could do that again, but I was very gratified
to find that Charles Gaba at _ACA Signups_ (odd name for a blog!) had done 
this <sup id="fn8a">[[8]](#fn8)</sup>, and at the county level to boot!  (All 3100+
counties in the US, which is&hellip; _special_.)  

Here's what his regression of % of total population vaccinated vs Trump/Biden popular vote
margin looks like:  

![Gaba: Vaccination level vs Trump margin, county-level data]({{ site.baseurl }}/images/2021-07-06-vaccinations-vs-votes-county-regression.jpg "Gaba: Vaccination level vs Trump margin, county-level data")  

Each data point is a county.  Those further to the right voted for Trump, while those
further to the left voted for Biden.  The higher points had more vaccination, while the
lower ones had less.  Note that each axis goes from 0% &ndash; 100%, so there's no
suspicious zooming in to make small effects look larger; this is the whole picture.  

Note the negative sloping trend: Trump counties did _terribly worse_ on vaccination
levels!  The regression line confirms this:  
- The negative slope of the line is -0.4224.  That is, for every 1% increase in Trump
  voters, there's a little under half a percent decrease in vaccination rates.  
- The model explains $R^2 \sim 42\%$ of the variance in the data, which is about as good as models
  like this ever get.  _Trumpiness is a good explainer of vaccine resistance._  
- Note the horizontal line at 85% vaccination: he's estimating this as the level of
  vaccination (or previous infection) required for herd immunity.  From that, we infer
  that he thinks COVID-19 has $R_0 \sim 6$ or so.  This is apparently based on some data
  from the Yale School of Medicine. <sup id="fn9a">[[9]](#fn9)</sup>  I'd have thought
  that a bit high, but the Delta (and Delta+) variants are a bit more virulent.  For once
  I'm _insufficiently_ pessimistic!  
- __Important point:__ _Nobody is yet at herd immunity!_  This means the unvaccinated _cannot_
  walk around hoping to be protected by the vaccinated around them.  

Since the population of unvaccinated is slowly shrinking, but the case rate is leveling
off, that means the rate of infection of unvaccinated people is going up.  If you're
unvaccinated, this should _terrify_ you.  (But if you're vaccinated, relax for now:
especially the mRNA vaccines work against all current variants.)  

So basically: there are a lot of knuckleheads refusing to get vaccinated for incredibly
stupid reasons.  They risk their own lives, sure.  But more importantly, they are
volunteering their bodies as collaborators in the war against COVID by being factories for
new variants.  

Sooner or later, one of those variants will escape our current vaccines.  And do you know
what happens then?  We start _all over again_, having to re-vaccinate _everybody_.  And I
mean _everybody_, planet-wide, not just in the US.  

All over again.  

It was hard the first time, even when we played nice and just asked people to accept a
free vaccine.  Next time, we probably won't play nice, and will have to use
[_Jacobson v Massachusetts_](https://en.wikipedia.org/wiki/Jacobson_v._Massachusetts)
to impose a vaccination mandate.  


## The Weekend Conclusion  

What to do?  Honestly, I just don't know.  

Ever since Reagan, the Republicans in the US have become increasingly irrational.  Today,
they're more or less fact-proof.  

How do you persuade a fact-proof knucklehead to do the right thing for the safety of
_everybody_, when they'd rather believe the vaccine is a plot by Bill Gates to implant a
chip so the government can reprogram them by 5G?  (Not an exaggeration!)  

Thanks, Republicans.  If not for you, we could have been more or less over COVID-19 in the
US by now.  But you're acting as though you _want_ a variant that'll make us do this all over
again.  Why would you possibly want that?!  

---

## Notes &amp; References  

<!--
<sup id="fn1a">[[1]](#fn1)</sup>
<a id="fn1">1</a>: [↩](#fn1a)  
-->

<a id="fn1">1</a>: Weekend Editor, ["Politics vs mask use & vaccine uptake in the US"](https://www.someweekendreading.blog/politics-vs-mask-and-vaccine-use/), [_Some Weekend Reading_ blog]({{ site.baseurl }}/), 2021-Apr-19. [↩](#fn1a)  

<a id="fn2">2</a>: Weekend Editor, [Omnibus dataset of state popular vote and vaccine usage]({{ site.baseurl }}/assets/2021-04-19-politics-vs-mask-and-vaccine-use-omnibus.tsv), from ["Why did Republicans block a Trump impeachment guilty verdict?"](https://www.someweekendreading.blog/republican-impeachment-votes/), [_SomeWeekendReading_ blog]({{ site.baseurl }}/), 2021-Feb-24. [↩](#fn2a)  

<a id="fn3">3</a>: Weekend Editor, ["JnJ Revenant"]({{ site.baseurl }}/jnj-revenant/), [_SomeWeekendReading_ blog]({{ site.baseurl }}/), 2021-Apr-23.[↩](#fn3a)  

<a id="fn4">4</a>: Weekend Editor, ["Another study of clotting and COVID vaccines"]({{ site.baseurl }}/covid-vaccines-and-clots/), [_SomeWeekendReading_ blog]({{ site.baseurl }}/), 2021-Apr-16.[↩](#fn4a)  

<a id="fn5">5</a>: Weekend Editor, ["US pauses JnJ vaccine on thromboses"]({{ site.baseurl }}/jnj-thrombosis-pause/), [_SomeWeekendReading_ blog]({{ site.baseurl }}/), 2021-Apr-13.[↩](#fn5a)  

<a id="fn6">6</a>: Weekend Editor, ["The AstraZeneca/Oxford Vaccine vs Blood Clots"]({{ site.baseurl }}/azox-vaccine-thrombo/), [_SomeWeekendReading_ blog]({{ site.baseurl }}/), 2021-Mar-17.[↩](#fn6a)  

<a id="fn7">7</a>: Weekend Editor, ["The Billionth Dose"]({{ site.baseurl }}/billionth-dose/), [_SomeWeekendReading_ blog]({{ site.baseurl }}/), 2021-Apr-24.[↩](#fn7a)  

<a id="fn8">8</a>: C Gaba, [Happy Independence Day. Here's U.S. &#x23;COVID19 Vaccination Levels BY COUNTY](https://acasignups.net/21/07/04/happy-independence-day-heres-us-covid19-vaccination-levels-county), [_ACA Signups_](https://acasignups.net/), 2021-Jul-04.[↩](#fn8a)  

<a id="fn9">9</a>: C MacMillan, ["Herd Immunity: Will We Ever Get There?"](https://www.yalemedicine.org/news/herd-immunity), [_Yale School of Medicine News_](https://www.yalemedicine.org/news/herd-immunity), 2021-May-21.[↩](#fn9a)  