| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Critique & Redesign: Visualizing Global Tomato Production

## The Original visualization
<img width="234" height="228" alt="截屏2025-09-18 上午1 09 51" src="https://github.com/user-attachments/assets/d8c44f02-533d-4c26-9221-cf9f295d7163" />

https://www.linkedin.com/feed/update/urn:li:activity:7038221922265915394/ 

## The critique
- **Usefulness**: Shows rankings clearly, but misses actual production scale.  
- **Completeness**: Title too vague; donut chart unexplained; no time range.  
- **Perceptibility**: Animation is engaging, but colors and background distract.  
- **Truthfulness**: Ranking-only view hides the huge gap between countries.  
- **Intuitiveness**: Flags are familiar, but icon-to-rank system is confusing.  
- **Aesthetics**: Dynamic and colorful, but overly saturated and messy.  
- **Engagement**: Strong animation and motion keep attention.
  
## Redesign Brainstorming

When I first started thinking about my redesign, I knew I wanted to use a map to show tomato production, since agriculture is deeply tied to geography. But I also wanted the visualization to feel more playful and personal, with a design language that connects to my earlier work. I recalled my previous Debt-to-GDP Red-Flag by Country (1995–2019) project, where I used small red dots to represent “red flags.” Visually, those red flags reminded me of little tomatoes, and I began to wonder if I could use tomato icons directly on the map as a way to show production quantities. So my first idea was to build a kind of density map, where tomatoes would tile across each region almost like population density. However, this approach quickly became too complex. It would require latitude/longitude points for each unit, and even if I solved the technical challenge, the result would likely be too cluttered and unreadable, especially since production values are measured in the millions of tons. Clearly, I couldn’t just place millions of tomato icons.

<img width="370" height="111" alt="截屏2025-09-18 上午2 27 39" src="https://github.com/user-attachments/assets/d96e43e3-08e3-4f68-a816-efa538cedfb7" />

## My tomato drawing: 

<img width="267" height="183" alt="截屏2025-09-18 上午1 13 13" src="https://github.com/user-attachments/assets/c55a93aa-80d3-42fe-bf51-173250b8d2a4" />

## First Design(Rank-Based Tomatoes)

So I considered a different strategy and come up with my first deisgn. I tried to tie the number of tomatoes to rank. For example, the top-ranked country could have 10 tomatoes, and the tenth-ranked country just 1. 

<div class='tableauPlaceholder' id='viz1758169053343' style='position: relative'><noscript><a href='#'><img alt='Global Tomato Production Ranking By Country｜1981-2021 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;2K&#47;2KY6GRB85&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='path' value='shared&#47;2KY6GRB85' /> <param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;2K&#47;2KY6GRB85&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1758169053343');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

At first this seemed like a neat simplification, but after reflecting and getting feedback from my interviewees, I realized this ranking system was misleading. The number of tomatoes became inversely tied to the rank number (rank 1 = 10 tomatoes, rank 10 = 1 tomato), which confused people. More importantly, it completely failed to show the real scale of differences. For instance, China is far ahead of the second-place country, producing five to six times more tomatoes, but my rank-based system would only show one extra tomato—an inaccurate and unhelpful signal.

## Incorporating Feedback into the Final Visualization
| Question | Interview 1 | Interview 2 |
|----------|-------------|-------------|
| Can you tell me what you think this is? | Said they quickly realized it was showing rankings, but it wasn’t obvious right away. | Recognized it as a ranking display, but pointed out that it doesn’t clarify the actual scale of production. |
| Can you describe to me what this is telling you? | Understood that more tomatoes = higher rank, but noted the logic is inverted (rank 1 has the most tomatoes, rank 10 the fewest), which caused some confusion. | Said the chart shows the top producers, but emphasized that the tomato counts don’t match the true production gaps. |
| Is there anything you find surprising or confusing? | Found it misleading that 9 tomatoes (2nd place) vs. 4 tomatoes (7th place) looks like a “double” relationship, when in reality the production values are not proportional. | Pointed out the title was unclear — it doesn’t specify the time span or how many countries are being ranked, which makes the scope ambiguous. |

The key pattern in the feedback was confusion about the ranking metaphor. Viewers needed time to realize tomatoes represented rank, and the inverted logic made the meaning unclear. They also felt the title was vague and missing the timeframe.

## Final Design 

In rethinking the design, I moved away from ranking and instead set a scaling baseline of 1,000,000 tons per tomato icon. This approach made it possible to translate the large production values into a manageable number of tomatoes while still preserving proportional relationships. For example, China’s 66 million tons are represented by 66 tomato icons, making the scale difference immediately visible compared to smaller producers. In developing this redesign, I relied on both Stephen Few’s critique criteria and the Good Charts framework, which highlighted key weaknesses of the original bar-race design: the lack of geographic context, the vague and misleading title, and the distracting background. My solution addresses these problems by situating production within its natural geography, using a clearer metaphor, and presenting the data with a cleaner, more perceptible aesthetic. Finally, to emphasize the temporal aspect of the data, I used Tableau’s Pages function so the visualization plays year by year, allowing viewers to watch global tomato production evolve over time.

<div class='tableauPlaceholder' id='viz1758177844033' style='position: relative'><noscript><a href='#'><img alt='Global Tomato Production by Country｜1981-2021Each 🍅 represents 1,000,000 tons                                                                                                          Faostat. Accessed September 18, 2025. https:&#47;&#47;www.fao.org&#47;faostat&#47;en&#47;# ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Gl&#47;GlobalTomatoProductionbyCountry1981-2021&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='GlobalTomatoProductionbyCountry1981-2021&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Gl&#47;GlobalTomatoProductionbyCountry1981-2021&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-CN' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1758177844033');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>


## References
/

## AI acknowledgements
_If you used AI to help you complete this assignment (within the parameters of the instruction and course guidelines), detail your use of AI for this assignment here._

