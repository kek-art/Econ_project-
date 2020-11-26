
## Problem Statement 

Proponents of art claim that it has several intangible benefits for communities invest in it. They claim art has the power to “transform minds, boost civic pride, improve mental and emotional wellbeing and instill hope in all citizens.”  But do these intangible effects actually translate into quantitative measures? In other words, is the impact of art limited to an internal experience or does it have a measured effect on communities and society? 


## Background 

Violent crime in the United States has seen a sustained drop over the last two decades.  The causes of this drop “are still largely unknown.”  However, it is largely agreed that there are several neighborhood-level risk factors that can contribute to violent crime such as “poverty rates, residential mobility, ethnic heterogeneity, and weak social networks.”  There is some evidence that art can help combat some of the driving forces behind violent crime. This evidence comes primarily from research focused on “individual-level effects of arts intervention programs on high-risk or justice-involved population, with the bulk of the literature focusing on youth.”  This does not prevent proponents of arts programs from touting art and performances as “effective ways to prevent or reduce crime.”   


## Data 
### Bureau of Labor Statistics (BLS)
1. newest: the average number of new independent art, writing, and performance establishments per 1,000 people 
1. avgempl: the annual number of persons employed as independent artists, writers, and performers per 1,000 people
### County Health Rankings (CHR)
1. violentcrime: is the number of reported crime offenses for 100,000 of the population
1. medianhouseholdincome: median income at the county level per year
1. highschoolgraduation: percentage of the ninth-grade cohort that graduates from high school in four years
1. unemployment: rate of population over 16 not currently employed but looking for employment
1. foodinsecurity: rate of households that experience “a lack of access, at times, to enough food for an active, healthy life for all household members and limited or uncertain availability of nutritionally adequate foods
1. severehousingproblems: percentage of households with one or more of the following problems: lacking complete kitchen facilities, plumbing facilities, overcrowding, or severely cost burdened
1. socialassociations: number of membership associations per 10,000 population
1. nonhispanicafricanamerican, hispanic and nonhispanicwhite: percentage breakdowns of ethnicity in a population
## Methodology 

I constructed a panel of county-level data and applied several regression models to the data in order to get a better understanding of the statistical association between arts employment and county violent crime rates. 

1. Scatter
  1. Observe a small negative correlation (see visualizing key results) 
1. Hausman 
    1. I rejected the random effects model because there was evidence that the difference between counties were correlated with the independent variables 
1. Fixed Effects 
    1. Just Employment
    1. Just Establishments 
    1. Both Employment and Establishments 

## Visualizing Key Results 

### Scatter Plots by Year Colored by FIPS Code 

<div class='tableauPlaceholder' id='viz1606085792972' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Da&#47;DataVisualization_16058059422160&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='DataVisualization_16058059422160&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Da&#47;DataVisualization_16058059422160&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en' /></object></div>              



<script type='text/javascript'>                    var divElement = document.getElementById('viz1606085792972');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.minWidth='420px';vizElement.style.maxWidth='650px';vizElement.style.width='100%';vizElement.style.minHeight='587px';vizElement.style.maxHeight='887px';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.minWidth='420px';vizElement.style.maxWidth='650px';vizElement.style.width='100%';vizElement.style.minHeight='587px';vizElement.style.maxHeight='887px';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else { vizElement.style.width='100%';vizElement.style.height='777px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>


### Heat Map of Violent Crime 


<div class='tableauPlaceholder' id='viz1606085814070' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Da&#47;DataVisualization2_16058063879810&#47;Dashboard2&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='DataVisualization2_16058063879810&#47;Dashboard2' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Da&#47;DataVisualization2_16058063879810&#47;Dashboard2&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en' /></object></div>             


<script type='text/javascript'>                    var divElement = document.getElementById('viz1606085814070');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.minWidth='420px';vizElement.style.maxWidth='650px';vizElement.style.width='100%';vizElement.style.minHeight='587px';vizElement.style.maxHeight='887px';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.minWidth='420px';vizElement.style.maxWidth='650px';vizElement.style.width='100%';vizElement.style.minHeight='587px';vizElement.style.maxHeight='887px';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else { vizElement.style.width='100%';vizElement.style.height='877px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

### Fixed Effects Regression Output 
![Fixed Effects]() 
![Random Effects]

## Policy Implications and Conclusion 

Based on my research there is no relationship between arts employment and violent crime. I think this is because art is a difficult concept to measure. 
1. The data I used only captured the number of people employed formally in the arts as “independent artists, writers, and performers.” Much of art happens informally, and the data from the BLS only captures full time employment. 
2. Does not capture part-time community arts programs, public art, or people who work in art-related-fields such as museum curators and educators.
### Further Research 
My research found no relationship between arts employment and violent crime and thus I cannot make any policy recommendations at this time. However, further research should be conducted using other measures such as number of public arts projects or community investment in the arts. 
