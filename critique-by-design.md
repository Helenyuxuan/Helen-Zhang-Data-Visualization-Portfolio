| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Critique & Redesign: Visualizing Global Tomato Production

## The Original visualization
https://www.linkedin.com/feed/update/urn:li:activity:7038221922265915394/ 
<img width="234" height="228" alt="截屏2025-09-18 上午1 09 51" src="https://github.com/user-attachments/assets/d8c44f02-533d-4c26-9221-cf9f295d7163" />


## The critique
- **Usefulness**: Shows rankings clearly, but misses actual production scale.  
- **Completeness**: Title too vague; donut chart unexplained; no time range.  
- **Perceptibility**: Animation is engaging, but colors and background distract.  
- **Truthfulness**: Ranking-only view hides the huge gap between countries.  
- **Intuitiveness**: Flags are familiar, but icon-to-rank system is confusing.  
- **Aesthetics**: Dynamic and colorful, but overly saturated and messy.  
- **Engagement**: Strong animation and motion keep attention.
  
## Building the Visulization

When I first started thinking about my redesign, I knew I wanted to use a map to show tomato production, since agriculture is deeply tied to geography. But I also wanted the visualization to feel more playful and personal, with a design language that connects to my earlier work. I recalled my previous Debt-to-GDP Red-Flag by Country (1995–2019) project, where I used small red dots to represent “red flags.” Visually, those red flags reminded me of little tomatoes, and I began to wonder if I could use tomato icons directly on the map as a way to show production quantities. So my first idea was to build a kind of density map, where tomatoes would tile across each region almost like population density. However, this approach quickly became too complex. It would require latitude/longitude points for each unit, and even if I solved the technical challenge, the result would likely be too cluttered and unreadable, especially since production values are measured in the millions of tons. Clearly, I couldn’t just place millions of tomato icons.

## My tomato drawing: 
<img width="109" height="105" alt="截屏2025-09-18 上午12 23 36" src="https://github.com/user-attachments/assets/ec9590f0-feba-4fea-8ff1-22eed25bdfce" />
<img width="299" height="240" alt="截屏2025-09-18 上午1 06 11" src="https://github.com/user-attachments/assets/5f231052-e686-4ec5-85da-3e3012bd6933" />

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
| **Can you tell me what you think this is?** | Said they quickly realized it was showing rankings,<br> but it wasn’t obvious right away. | Recognized it as a ranking display,<br> but pointed out that it doesn’t clarify the actual scale of production. |
| **Can you describe to me what this is telling you?** | Understood that more tomatoes = higher rank,<br> but noted the logic is inverted (rank 1 has the most tomatoes,<br> rank 10 the fewest), which caused some confusion. | Said the chart shows the top producers,<br> but emphasized that the tomato counts don’t match the true production gaps. |
| **Is there anything you find surprising or confusing?** | Found it misleading that 9 tomatoes (2nd place)<br> vs. 4 tomatoes (7th place) looks like a “double” relationship,<br> when in reality the production values are not proportional. | Pointed out the title was unclear — it doesn’t specify the time span<br> or how many countries are being ranked, which makes the scope ambiguous. |

## Synthesis
The key pattern in the feedback was confusion about the ranking metaphor. Viewers needed time to realize tomatoes represented rank, and the inverted logic made the meaning unclear. They also felt the title was vague and missing the timeframe.

Based on this, I rethought the design. Instead of using rank, I decided to set a scaling baseline of 1,000,000 tons per tomato icon. This way, I could translate the large production values into a manageable number of tomatoes while still keeping the proportional relationships correct. For example, China’s 66 million tons would be shown as 66 tomatoes, while smaller producers would naturally display fewer.
Throughout this process, I found that combining Stephen Few’s critique criteria with the Good Charts framework helped me identify specific weaknesses in the original bar-race design: the lack of geographic context, the vague and misleading title, and the distracting background. My redesign addresses these issues by situating production in its natural geographic context, using a clearer metaphor, and presenting the data with a cleaner, more perceptible aesthetic.

## Final Design (Scaled Tomatoes by Production)

For my final redesign, I created a map-based visualization of global tomato production, where each tomato icon represents 1,000,000 tons. This approach allowed me to directly tie the tomatoes to the data values, so that larger producers are represented by visibly more tomatoes. For example, China is shown with 66 tomato icons, clearly communicating the scale of its production compared to smaller producers. Also, the visualization uses Tableau’s Pages function so that the data plays year by year, allowing viewers to watch production change over time.


## References
/

## AI acknowledgements
_If you used AI to help you complete this assignment (within the parameters of the instruction and course guidelines), detail your use of AI for this assignment here._

