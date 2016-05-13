# 2016-05-12
May 2016 Meetup

Kate Ergle presents Tableau:

The talk will be about an important part that cannot be skipped when fitting models to your data - exploring the data set. The best way to do it is with interactive analysis. This can and needs to be done also when analyzing Big Data - the secret to that is random sampling. The emphasis in this talk will be on Tableau which is a business intelligence software that is not very complex but is very powerful.

Link to slides: https://docs.google.com/presentation/d/1xSvBROEHhjRkWaCTttn6x9bbZYTqZrwzIzFtUtYse1k/edit?pref=2&pli=1#slide=id.p

Tableau helps you choose a chart:
http://www.tableau.com/learn/whitepapers/which-chart-or-graph-is-right-for-you

Formula for CPA_color:

IF ISNULL(SUM([Regs])) THEN 5
ELSE IF (sum([Costs])/sum([Regs]) / [cpa_threshhold]) >= 5 THEN 5
ELSE (sum([Costs])/sum([Regs])) / [cpa_threshhold]
END
END
