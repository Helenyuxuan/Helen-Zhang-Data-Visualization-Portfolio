| [About Me](README.md) | [Gov Debt Viz](dataviz-examples.md) | [Whisky Viz](dataviz-examples-Whisky.md) | [Critique by Design](critique-by-design.md)| [Final Project I](final-project-part-one.md) | [Final Project II](final-project-part-two.md) | [Final Project III](final-project-part-three.md) |

## Assignment: [Visualizing overnment Debt](visualizing-government-debt)

This page presents my work for the *Visualizing Government Debt* assignment.  
I created several Tableau dashboards to explore how government debt has evolved across countries and over time.  

## Graph 1

<div class='tableauPlaceholder' id='viz1757094492546' style='position: relative'><noscript><a href='#'><img alt='Dashboard 3 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;De&#47;Debt-toGDPRed-FlagbyCountryThisisavisualrepresentationnotanacademicclaim&#47;Dashboard3&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Debt-toGDPRed-FlagbyCountryThisisavisualrepresentationnotanacademicclaim&#47;Dashboard3' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;De&#47;Debt-toGDPRed-FlagbyCountryThisisavisualrepresentationnotanacademicclaim&#47;Dashboard3&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-CN' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1757094492546');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  if ( divElement.offsetWidth > 800 ) { vizElement.style.width='1200px';vizElement.style.height='827px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='1200px';vizElement.style.height='827px';} else { vizElement.style.width='100%';vizElement.style.height='827px';}                     
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>


In my first version, I wanted to clearly show which countries exceeded 100% debt-to-GDP most frequently. I designed a two-panel view:

- Left: Total count of years each country’s debt-to-GDP reached or exceeded 100%.
- Right: A timeline of dots for each year (red indicates ≥100%, hollow gray indicates below 100%).

I used full country names on the left for clarity and three-letter codes on the right to save space. Below the title, I included a note: “≥100% is a visual cue, not a universal threshold,” to emphasize that this is a visual representation rather than an absolute economic benchmark.

Compared to a typical heatmap, this layout allows viewers to quickly identify the countries with the highest debt burden (left, sorted) while still showing when those high-debt years occurred (right, using dots). I also consolidated the legends to avoid redundancy.

 

## Graph 2

<div class='tableauPlaceholder' id='viz1757128120347' style='position: relative'><noscript><a href='#'><img alt='Dashboard 4 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;De&#47;Debt-to-GDPAcross34Countries19952019DistributionsMedianTrend&#47;Dashboard4&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Debt-to-GDPAcross34Countries19952019DistributionsMedianTrend&#47;Dashboard4' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;De&#47;Debt-to-GDPAcross34Countries19952019DistributionsMedianTrend&#47;Dashboard4&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-CN' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1757128120347');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  if ( divElement.offsetWidth > 800 ) { vizElement.style.width='1200px';vizElement.style.height='1127px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='1200px';vizElement.style.height='1127px';} else { vizElement.style.width='100%';vizElement.style.height='727px';}                     
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

This graph shows the yearly median debt-to-GDP ratio across the same 34 countries from 1995 to 2019. Each point represents the median value for that year (unweighted), and the y-axis is measured in percentage terms, with a reference line at 100% for context.

This graph shows the median debt level gradually declined through the mid-2000s, rose sharply after the 2008 financial crisis, remained elevated for several years, and then slightly decreased by 2019.

This second graph does not capture cross-country variation or account for differences in economic size, which is why the first dashboard remains useful for identifying which specific countries exceeded the threshold and when.


## References
**Data Source**: Organisation for Economic Co-operation and Development (OECD). *General Government Debt (Indicator)*.  
OECD Data. Accessed September 4, 2025.  
[https://data.oecd.org/gga/general-government-debt.htm](https://data.oecd.org/gga/general-government-debt.htm)


## AI acknowledgements
I used ChatGPT to help correcting errors in my code, asking question about where to find bolding labels, adjusting alignment, and resizing icons.

[Back to Main Page](README.md)
