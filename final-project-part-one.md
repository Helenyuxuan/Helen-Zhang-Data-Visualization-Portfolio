| [About Me](README.md) | [Gov Debt Viz](dataviz-examples.md) | [Whisky Viz](dataviz-examples-Whisky.md) | [Critique by Design](critique-by-design.md)| [Final Project I](final-project-part-one.md) | [Final Project II](final-project-part-two.md) | [Final Project III](final-project-part-three.md) |

# Visualizing Allegheny County’s Birds in Sound and Space - Final Project Part I 
## Outline

This project frames the Allegheny County’s birds through sound and space, offering windows into their habits and habitats. By visualizing five common species across both their calls and their places, the project creates a more accessible way to get closer to these birds.

I chose this topic because listening to birds has always felt both familiar and calming for me. When I hear a robin or cardinal outside my window, I notice the rise and fall of their notes, but I cannot confidently say which bird is which. That uncertainty made me curious: could visual translation bridge the gap between what we hear and what we know? My goal is to create a set of data visualization that highlights not only the shape of a single bird song but also the variety within each species.

To achieve this, the project does not rely on pre-made spectrogram images but instead begins with the raw sounds themselves. Each recording is broken down into thousands of individual points that capture time, frequency, and intensity, and these points are then reconstructed in Tableau. The result looks similar to a spectrogram, but it is a dataset-driven visualization that can be filtered, reshaped, and directly compared. This approach makes the act of listening more accessible—moving away from a static format meant for specialists and toward a visual form that is open to a broader audience.

From there, the points are organized into distinct “singing styles,” such as the clear notes of a Phrase, the rapid repetitions of a Series, the fluid tones of a Warble, and the quick, even beat of a Trill. These categories, drawn from Nathan Pieplow’s framework for describing birdsong patterns (Pieplow 2009), provide a bridge between technical audio data and a more intuitive, musical understanding. Beyond single examples, the project also works on two levels of comparison: across species, where Allegheny County’s five common birds can be set side by side; and within species, where different song types are separated and displayed to reveal the richness and variation of a single voice.

Paired with maps that show where these birds are found in Allegheny County, the project brings together sound and place, hearing and seeing. It is an invitation to slow down, pay attention, and discover how much life is carried in the voices around us. By using data visualization to uncover the hidden patterns within these songs, I hope to encourage a deeper connection to the natural world that exists right outside our windows.

## One-Sentence Summary

My story aims to demonstrate how the songs of Allegheny County’s most common birds can be transformed from fleeting sounds into visual data, making it easier for people to see differences, identify species, and understand where these birds live.

## User Stories

This project is designed for audiences who want to connect sound with species and place in an accessible way. A casual listener may want to identify which bird is singing outside their window, while a beginner birder may look to compare different singing styles across species. Local residents may explore maps to see where these birds are found in Allegheny County, linking calls to familiar locations. At the same time, educators and science communicators may use the project as a visual dictionary of birdsongs that translates technical spectrogram data into forms that the broader public can understand.

## Story Arc

<img width="2752" height="2064" alt="未命名作品 2" src="https://github.com/user-attachments/assets/99161549-986a-41be-9218-3d20cc4f7a56" />

## Storyline (logic of the sketch)

- **From whole to part:** begin with a map of Allegheny County showing bird distributions  
  (different colors = different species).  

- **Focus on one bird:** extract a single species from the map and enlarge its points.  

- **Song comparison:** based on these points, show the different song categories of that species  
  (*Phrase / Series / Warble / Trill*), allowing the audience to see its “vocal diversity.”  

- **Movement path:** also mark the activity route of this bird/this species,  
  showing its movement or distribution changes over time.  

- **Next step (to be continuous):** possibly extend to habits or migration routes (still in progress).  


## Initial sketches


<img width="977" height="544" alt="截屏2025-09-25 下午10 24 27" src="https://github.com/user-attachments/assets/7b0eca67-246b-4645-be40-79d5a35dda20" />

<img width="984" height="469" alt="截屏2025-09-25 下午10 27 13" src="https://github.com/user-attachments/assets/a88eb36c-9f42-4c8c-84cf-a8e36c73da88" />


<img width="936" height="541" alt="截屏2025-09-25 下午10 30 54" src="https://github.com/user-attachments/assets/b8cdabf6-256d-4fdd-b70a-f6bf2d60bb3e" />

# The data

For this project, I am working with two complementary types of data: bird observation records and birdsong recordings.

The first source comes from eBird, which provides the eBird Basic Dataset (EBD). By filtering the data to Allegheny County and surrounding Allegheny County, I can identify the five most common bird species and map where they appear most frequently. Each record includes species, location, date, and effort details, which makes it possible to visualize distribution patterns at a local scale.

The second source comes from the Macaulay Library, specifically The Cornell Guide to Bird Sounds: United States and Canada. This guide is a curated collection of high-quality field recordings that represent a wide range of vocalizations for North American birds. By using these recordings, I can create datasets of time, frequency, and amplitude for each song. Instead of leaving them as static spectrogram images, I reconstruct each sound into thousands of individual points. This method allows me to compare calls interactively, group them into categories (Phrase, Series, Warble, Trill), and explore variation both across and within species.

Together, these datasets allow me to connect sound and place: eBird records ground the birds in Allegheny County’s geography, while the Macaulay Library recordings reveal the acoustic diversity of their songs. By linking them, I can build a more complete story that moves between hearing, seeing, and mapping.


| Name | URL | Description |
|------|-----|-------------|
|eBird Basic Dataset (EBD)| https://ebird.org/data/download/ebd|Global citizen-science dataset of bird observations, filtered to Allegheny County for this project. Includes species, date, and coordinates.|
|Macaulay Library – The Cornell Guide to Bird Sounds: United States and Canada|https://www.macaulaylibrary.org/product/the-cornell-guide-to-bird-sounds-us-and-canada/|A curated collection of bird songs and calls from across North America. Used as the primary source for Allegheny County’s five common species in this project.|
|      |     |             |

# Method and medium

I will complete this project by combining signal processing with data visualization. First, I process raw bird recordings in Python using librosa, converting each sound into thousands of data points that capture time, frequency, and intensity. These datasets are then imported into Tableau, where I reconstruct them into visual forms that resemble spectrograms but allow for filtering, reshaping, and side-by-side comparison. To connect the visualizations back to everyday experience, I will organize examples into distinct singing styles and map their occurrence across Allegheny County using eBird data. The final product will be an interactive, web-based story presented through a GitHub site, integrating Tableau dashboards, narrative text, and supporting sketches to guide the audience from listening to seeing.

<img width="1170" height="290" alt="截屏2025-09-25 上午12 06 55" src="https://github.com/user-attachments/assets/c5c4af73-084b-4293-afda-7f77456cfa48" />

**Step 4. Reconstruct in Tableau （Demo）**
Import the CSV file into Tableau and plot it with Time (s) on the x-axis, Frequency (Hz) on the y-axis, and dB (intensity) mapped to size or color. This step rebuilds the sound into a point-based visualization that resembles a spectrogram but remains flexible: it can be filtered, zoomed, and reshaped to highlight particular song types. The demo shown here displays the Louisiana Waterthrush (Series) pattern, reconstructed directly from the exported dataset.
<div class='tableauPlaceholder' id='viz1758772228338' style='position: relative'><noscript><a href='#'><img alt='Louisiana Waterthrush Sound |SERIES| ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Lo&#47;LouisianaWaterthrushSoundSERIES&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='LouisianaWaterthrushSoundSERIES&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Lo&#47;LouisianaWaterthrushSoundSERIES&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-CN' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1758772228338');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

## Possible Design Style

Instead of a traditional science graphic, I want the project to feel more like a sketchbook or field journal. The visuals will mix sound-derived data points with sketch-like elements, creating a style that is playful and exploratory rather than purely explanatory. This approach makes the project more inviting for a broader audience, balancing scientific rigor with artistic curiosity.

## References

Pieplow, Nathan. 2009. “The Four Basic Patterns of Repetition and Speed.” Earbirding. October 21, 2009. https://earbirding.com/blog/specs/the-four-basic-patterns-of-repetition-and-speed.

**Data**

eBird. 2025. eBird Basic Dataset (EBD). Cornell Lab of Ornithology. Accessed September 24, 2025. https://ebird.org/data/download/ebd.

Macaulay Library. 2025. The Cornell Guide to Bird Sounds: United States and Canada. Cornell Lab of Ornithology. Accessed September 24, 2025. https://www.macaulaylibrary.org/product/the-cornell-guide-to-bird-sounds-us-and-canada/.

## AI acknowledgements
I used ChatGPT to help correcting errors in my code.
