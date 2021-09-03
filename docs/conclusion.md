# Conclusion

The problem is: `How do annual members and casual riders use Cyclistic bikes
differently?`. The stakeholders involved in this problem are Lily Moreno, the
director of marketing and my manager, the marketing team that is interested in
helping the company and the executive team that will decide whether to approve
the marketing program. To make it more effective to convey the result of the
program to the stakeholders I must take into account the fact that:

- the executive is detail-oriented
- the marketing team needs to better understand how annual members and casual
  riders differ, why casual riders would buy a membership, and how digital
  media could affect their marketing tactics.
- and the manager is responsible for the the development of the marketing
  campaigns.

Also, I've tried to do this exercise by following a few conventions, such as
file structure (cookiecutter data science template that I adapted to the R
project) and filling out different R notebooks for different steps. The report
is also a separate file to allow export to other formats such as PDF and HTML.

(For this case study, the data was supplied as if being data collected by the
company itself so I will follow that roleplay.)

The data was collected by the company itself during the last year. It is
organized by month, ranging from 2020-04 to 2021-05. The data is standardized -
I assume it was collected by using sensors on the bikes themselves and also the
whole subscription software system that handles all the data about the users
and the bikes. I will also assume that there are no problems with bias as the
data is about all the bikes and users - not a sample - and finding out if the
product itself is biased towards a specific type of user is a problem outside
of this case study.

I split the cleaning in two steps: merging and cleaning. The first step is
merging the data of the different months into a single dataset and the second
step is about ensuring that there are no missing data, wrongly typed membership
status, bike types. Also, I've calculated the trip duration and the distance
traveled (by using the latitude and longitude). This two new columns will help
on filtering/fixing errors about dates and distances.  Data that had dates and
longitude and latitude data missing were removed.

This is what I found about the data:

- almost 60% of users have a `membership status`
- the most used bike is the `docked bike`
- in terms of distance, both users do around 1km
- in terms of time traveled, the `casual` user spends about 20 minutes and the
  `member` user spends about 11 minutes
- there are more `casual` users at weekends
- `members` use bikes throughout the week - I assume that they are commuting
- there are more users (both members and casuals) during the summer, more
  specifically July - October
- `casuals` travel more distance on October-January and members travel more
  distance on July - October

All the graphs I've made are standard graphs used in analysis:
- bar
- line
- box-plot
- histogram.

I'm not proud of any of the graphs as there isn't anything new, but the last
graphs I've made pointed me to consider about COVID-19 as the lows coincide
with the periods of confinement of the pandemic.

Honestly, I don't know what to recommend. I don't have enough information nor
experience to know what should be done in this case. To make matters worse, the
fluctuations in users and distance/time traveled also change accordingly to the
COVID-19 fluctuations. Before writing any conclusions I would have to speak
with the manager and the team before arriving at any conclusion. This
particular situation isn't something I alone can manage. I don't have enough
information.
