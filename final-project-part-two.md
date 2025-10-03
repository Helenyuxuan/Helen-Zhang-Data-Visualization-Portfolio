| [About Me](README.md) | [Gov Debt Viz](dataviz-examples.md) | [Whisky Viz](dataviz-examples-Whisky.md) | [Critique by Design](critique-by-design.md)| [Final Project I](final-project-part-one.md) | [Final Project II](final-project-part-two.md) | [Final Project III](final-project-part-three.md) |

# Wireframes / storyboards
My storyboard lays out the progression of the project in a clear, sequential way. The narrative begins with a county-wide overview, using bar charts to identify the five most frequently observed bird species in Allegheny County. From there, the story narrows in on each individual species. For the Northern Cardinal, which I have developed first(TOP 1 observed bird), the section includes a brief introduction, a location map showing where it is most often recorded, and a visualization of its songs that reconstructs the sound as data points in Tableau.

The full project will apply this same structure to all five species, ensuring that each one is represented with consistent visual elements: an introduction, a distribution map, and a visualization of song styles. There will be additional visualization that show changes in recorded observations across seasons and years, connecting individual birds back to larger ecological patterns.

This storyboard structure is logically presented, moving from the broad (all county records) to the specific (individual birds), and it provides a sufficient number of visualizations to tell a compelling story. By adopting a sketchbook-like style, the project makes bird data approachable for casual audiences, including birdwatchers, students, or local residents, so the visuals do not just inform but invite curiosity. This combination of outline, draft data visualizations, and audience framing meets the requirements for a clear, engaging storyboard.

## Design: data visualizations

For this project, I have identified several key visualizations that will guide the reader through the story of Alle’s five most common birds. Each visualization is designed to connect sound, space, and species, making the patterns of birdsong more intuitive and engaging. All datasets are restricted to the period **2015–2025 (present)** to ensure both recency and consistency.  

- **Top 5 Most Observed Species (Bar Chart)**  
  A bar chart ranking the five most commonly observed bird species in Allegheny County. This sets the stage by establishing which species are most present in daily life.
<img width="648" height="310" alt="截屏2025-10-02 下午6 56 56" src="https://github.com/user-attachments/assets/5ce701c8-94cb-460c-8a66-029271f20be3" />

**Using the Northern Cardinal as an example, the other four species will follow the same format.**

- **Species Profile: Northern Cardinal (Sample Page)**
A focused profile that blends text, imagery. Features a short descriptive narrative, scientific details, and a clear visual identity (color, photo, or icon).
<img width="725" height="426" alt="截屏2025-10-02 下午6 59 57" src="https://github.com/user-attachments/assets/42917b53-a045-404c-b989-7a6dc05afbdc" />

**Note:** Explanations of bird sound visualization categories (e.g., **trill**, **series**, **musical vs. non-musical tones**...) are based on resources from *Earbirding* (Earbirding, *The Four Basic Patterns of Repetition and Speed*).

- **Species Distribution Map (Map in Tableau)**  
  A map showing where each species has been recorded across Allegheny County. Different colors represent different species, giving a geographic context to where these birds can be found.

<img width="647" height="396" alt="截屏2025-10-02 下午6 59 37" src="https://github.com/user-attachments/assets/d98ad762-46f8-4e7c-9a54-777aff7ddb6c" />

- **Still deciding to include or not :Yearly Observation Trends (Line Chart)**  
A time-series view of reported observations across years. While this doesn’t directly measure population size—since the same bird can be observed multiple times—it matters because it shows when and how people most often encounter these birds. The rhythm of reporting reflects both the birds’ seasonal activity and our habits of noticing them. This temporal perspective sets the stage for sound visualizations, where we shift from when we see them to how we hear them.


<img width="403" height="384" alt="截屏2025-10-02 下午7 29 44" src="https://github.com/user-attachments/assets/ad61520a-806c-44a1-83ed-31a7d9551fd2" />


- **Song Visualization (Spectrogram-based Graphs)**  
  Each bird’s song is translated into a dataset of frequency, time, and intensity points, reconstructed in Tableau. These graphs make calls visible and allow comparisons across different song types within each species (Phrase, Series, Warble, Trill).

<img width="480" height="377" alt="截屏2025-10-02 下午7 02 56" src="https://github.com/user-attachments/assets/8f4880d3-00d0-4090-9806-b7ae5708be1f" />
<img width="556" height="373" alt="截屏2025-10-02 下午7 32 35" src="https://github.com/user-attachments/assets/daf5eaf8-82fe-47af-b239-a30995603b62" />

- **Still deciding to include or not: Individual Bird Tracking (Route Map)**
A visualization tracing the movement of a single bird (based on observer ID and repeated sightings). While not representative of the entire species, it offers a personal lens into the data—showing how one bird might weave through parks, rivers, and neighborhoods over time. This perspective makes the dataset feel more tangible, connecting scientific records to the lived landscapes where people encounter these birds.

<img width="468" height="270" alt="截屏2025-09-25 下午10 30 54" src="https://github.com/user-attachments/assets/b8cdabf6-256d-4fdd-b70a-f6bf2d60bb3e" />


# User Research  

## Target Audience  

The target audience for this project is the broader Allegeny community, particularly people who hear birds daily but do not necessarily recognize them by sound or appearance. This includes casual park visitors, city residents, and students or educators who want accessible, visual ways to learn about local bird species.  

To make the research representative, I identified three groups to focus on:  

1. **Beginner birdwatchers** – people who may notice birds but struggle to match calls with species.  
2. **Local residents** – individuals who encounter birds in parks and neighborhoods but usually treat them as background noise.  
3. **Curious learners** – students and educators interested in combining nature and data visualization in more playful, sketchbook-like ways.  

This choice ensures that the design of data visualizations—maps, song reconstructions, and observation trends—remains both accurate and approachable. Titles, annotations, legends, captions, and sources are added not only for precision but also to keep the project open and engaging for non-specialists.  


## Interview Script  

| Goal | Questions to Ask |  
|------|------------------|  
| Understand baseline familiarity with birds | When you hear birds around Allegheny County, do you usually notice or ignore them? |  
| Test clarity of visualizations | Looking at this visualization, can you tell what it represents without me explaining? |  
| Identify confusing elements | Is there anything here that feels too technical, overwhelming, or hard to follow? |  
| Measure engagement | Does this sketchbook-style presentation feel inviting, or would you prefer a more formal/scientific style? |  
| Evaluate narrative flow | Does the order—maps, profiles, songs, and trends—make sense to you? If not, how would you expect the story to flow? |  
| Explore personal connection | Do these visuals make you want to pay more attention to bird calls in daily life? |  


## Interview Findings  

- Interviewee 1: classmate (graduate student, 20s), 
- Interviewee 2: classmate (graduate student, 20s)
- Interviewee 3: birder friend outside of class (adult educator, 30s)

| Questions | Interview 1 | Interview 2 | Interview 3 |  
|-----------|-------------|-------------|-------------|  
| Do you usually notice or ignore bird sounds? | Notices but cannot identify; interested in “seeing” the sounds. | Usually ignores unless very loud. | Notices often and travel alot for bird watching and listening |  
| Can you tell what the visualizations represent? | Understood spectrogram shapes after explanation; suggested simpler labels. | Found some visuals confusing, especially the frequency axis. | Understood with annotations; appreciated the sketchbook tone. |  
| Is anything too technical or overwhelming? | Yes, scientific terms like “trill” need small definitions. | Charts without annotations feel “cold.” | Too much data on one screen could overwhelm students. |  
| Do you like the sketchbook style? | Yes, felt more personal than a report. | Yes, makes it playful and approachable. | Very positive, sees it as a teaching tool. |  
| Does the story flow make sense? | Yes, but wanted more transition text between sections. | Suggested starting with sound before maps. | Liked the flow but wanted seasonal context added. |  
| Would you pay more attention to bird calls after seeing this? | Yes, wants to try identifying them. | Yes, at least curious. | Definitely, would use with students. |  
| What would you change? | Add “legend” for sound types. | Reduce amount of text on one page. | Make seasonal variations clearer. |  


# Identified Changes for Part III  

Based on these interviews, I plan to make the following changes to improve clarity and engagement:  

| Research Synthesis | Anticipated Changes for Part III |  
|--------------------|----------------------------------|  
| Participants found spectrogram-style visualizations hard to interpret without guidance. | Add short annotations and legends (e.g., arrows marking “rising note” or “falling note”), keep terms simple, and cite source (Earbirding). |  
| Narrative transitions felt abrupt. | Write short, sketchbook-style transition notes between sections (e.g., moving from “where to find them” → “how they sound”). |  
| Seasonal context requested. | Add a seasonal/quarterly observation graph alongside yearly trends. |  
| Too much information at once could overwhelm. | Break visuals into smaller steps—first species maps, then song visualizations, then trends, instead of showing all together. |  
| Sketchbook style appreciated by all groups. | Keep the sketchbook tone; emphasize personal observations and hand-drawn feel in final design. |  


## Final Thoughts  

The user interviews confirmed that the playful sketchbook framing is a strong strength of the project, but the clarity of visualizations depends heavily on annotations and transitions. Moving forward, I will simplify technical language, build in seasonal perspectives, and ensure smoother narrative flow so that the story is inviting to both beginners and educators.  


## References
- eBird. *eBird Basic Dataset (EBD)*. Cornell Lab of Ornithology. Retrieved from: https://ebird.org/data/download  
- Macaulay Library. *The Cornell Guide to Bird Sounds: United States and Canada*. Cornell Lab of Ornithology. Retrieved from: https://www.macaulaylibrary.org/product/the-cornell-guide-to-bird-sounds-us-and-canada/  
- Earbirding. *The Four Basic Patterns of Repetition and Speed*. Retrieved from: https://earbirding.com/blog/specs/the-four-basic-patterns-of-repetition-and-speed  
- BirdLife International. *Northern Cardinal (Cardinalis cardinalis) species factsheet*. Retrieved from: https://datazone.birdlife.org/species/factsheet/northern-cardinal-cardinalis-cardinalis  
## AI acknowledgements
- Helped refine the clarity of project descriptions, correct the grammar of my sketchbook-style narrative writing
- Correct python and Github code for me


