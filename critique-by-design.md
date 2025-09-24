| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [Data Visualization - Government Debt](dataviz-examples.md) | [critique by design](https://github.com/Helenyuxuan/Helen-Zhang-portfolio/blob/main/critique-by-design.md) | [final project I](final-project-part-one.md) | [final project II](final-project-part-two.md) | [final project III](final-project-part-three.md) |

# Critique & Redesign: Visualizing Global Tomato Production

## The Original visualization
https://www.linkedin.com/feed/update/urn:li:activity:7038221922265915394/ 

<img width="234" height="228" alt="截屏2025-09-18 上午1 09 51" src="https://github.com/user-attachments/assets/d8c44f02-533d-4c26-9221-cf9f295d7163" />

This original design is a bar-race video showing changes in global tomato production rankings. It uses animated bars with country flags to highlight shifts over time, focusing mainly on rank order rather than production scale.

**Why I chose this visualization**:
- I chose this data visualization because agriculture, particularly tomato production, is a worldwide sector with significant regional variations. Tomatoes are among the most extensively consumed crops, and the graph shows how a few countries dominate production while others contribute on a smaller scale. This is a compelling case for investigating how data visualization might communicate both ranking and scale.
- I wanted to explore how the previous design tackled this topic and whether, if I were to rework it, I could present the facts more clearly by linking production to location and making scale disparities more intuitive.

## The critique

The data visualization is a bar-race chart showing the rankings of global tomato producers over time. The animation of bars growing and shrinking year by year is engaging, and the use of country flags makes it easy to connect the data to national identities. This design is effective for quickly showing which countries are leaders and how their rank changes across time.

However, there are several issues that reduce its effectiveness. The truthfulness is limited because viewers may expect larger producing countries to display proportionally more tomatoes, but the ranking format does not provide that information. The completeness is also weak: the title is vague, it does not specify the time span or number of countries included, and the donut chart on the side is left unexplained, making its meaning ambiguous. Finally, the perceptibility suffers from distractions: the photographic tomato background and overly saturated colors compete with the data, and the design feels more like advertising than analysis.

Taken together, these issues undermine clarity and accuracy, leaving the audience with only a partial and somewhat confusing understanding of global tomato production.

## Redesign Brainstorming

When I first started thinking about my redesign, I knew I wanted to use a map to show tomato production, since agriculture is deeply tied to geography. But I also wanted the visualization to feel more playful and personal, with a design language that connects to my earlier work. I recalled my previous Debt-to-GDP Red-Flag by Country (1995–2019) project, where I used small red dots to represent “red flags.” Visually, those red flags reminded me of little tomatoes, and I began to wonder if I could use tomato icons directly on the map as a way to show production quantities. 

<img width="370" height="111" alt="截屏2025-09-18 上午2 27 39" src="https://github.com/user-attachments/assets/d96e43e3-08e3-4f68-a816-efa538cedfb7" />

So my first idea was to build a kind of density map, where tomatoes would tile across each region almost like population density. However, this approach quickly became too complex. It would require latitude/longitude points for each unit, and even if I solved the technical challenge, the result would likely be too cluttered and unreadable, especially since production values are measured in the millions of tons. Clearly, I couldn’t just place millions of tomato icons.

## My tomato drawing: 

<img width="267" height="183" alt="截屏2025-09-18 上午1 13 13" src="https://github.com/user-attachments/assets/c55a93aa-80d3-42fe-bf51-173250b8d2a4" />

## Sketch a solution: First Design(Rank-Based Tomatoes)

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

**Synthesis**:

Overall, the feedback revealed a recurring issue with the ranking metaphor. Several viewers mentioned that it took them a few seconds to understand that the tomatoes were not decorative but actually represented rank. This delay in recognition, combined with the inverted logic of “more tomatoes = higher rank,” made the visualization less intuitive and risked confusing the audience. Another key point raised was that the title lacked specificity: it did not clearly state the time span of the data or the number of countries being ranked, which left the scope ambiguous. These gaps weakened both the clarity and completeness of the design.

Hearing these comments helped me realize that, while the ranking system simplified the data, it also hid the true differences in production scale. For example, the gap between the first and second producers is enormous, but the rank-based tomato counts made it appear minimal. In my redesign, I wanted to address this by moving away from rank as the main encoding and instead introducing a proportional measure that shows the actual production more clearly. I also plan to refine the title so that it sets up the timeframe and scope immediately, ensuring that viewers know what they are looking at from the very start.
## Final Design 

In rethinking the design, I began by questioning whether ranking was the best way to communicate tomato production. Although ranking simplifies the story, the feedback I received made it clear that it obscured the true scale of differences. For example, the gap between the first and second producers was enormous, yet the ranking system made it look small. This realization pushed me to look for a proportional system that could communicate both scale and comparison more directly.

The next step was to decide on a practical unit. Since production values are reported in millions of tons, I set a scaling baseline of 1,000,000 tons per tomato icon. This gave me a way to translate very large dataset into a visual form that audiences could grasp intuitively, while still preserving proportional relationships. For example, China’s 66 million tons became 66 tomato icons.

After setting the scale, I refined the map itself. I updated the map background to make geographic boundaries clearer, adjusted the labels so they were better aligned with country locations, and added country name annotations to reduce ambiguity. These changes made the visualization easier to navigate and more perceptible for viewers who may not be familiar with all regions. I also revised the title to explicitly state the timeframe and scope, so audiences could understand right away that the visualization covered global tomato production across 1981–2021.

Together, these adjustments created a design that is not only more truthful and complete, but also easier to interpret at a glance.


<div class='tableauPlaceholder' id='viz1758180543641' style='position: relative'><noscript><a href='#'><img alt='Global Tomato Production by Country｜1981-2021Each 🍅 represents 1,000,000 tons                                                                                            Faostat Accessed September 18, 2025. https:&#47;&#47;www.fao.org&#47;faostat&#47;en&#47;#data&#47;QCL.) ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Gl&#47;GlobalTomatoProductionbyCountry1981-2021&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='GlobalTomatoProductionbyCountry1981-2021&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Gl&#47;GlobalTomatoProductionbyCountry1981-2021&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-CN' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1758180543641');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>


## References
**Data Source**: Food and Agriculture Organization of the United Nations. FAOSTAT: Crops and Livestock Products. Accessed September 18, 2025. https://www.fao.org/faostat/en/#data/QCL.

## AI acknowledgements
I used ChatGPT to help correcting errors in my code, asking question about where to find bolding labels, adjusting alignment, and resizing icons.
