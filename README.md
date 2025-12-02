# Final Project
Link to actual repo (needed to unfork for lfs): https://github.com/saordoe/funny-fuel

## Project planning: Design Doc (due 11/5)
### Design Doc
#### Introduction
- We are motivated to make an immersive experience within a surreal procedural city.

#### Goal
- We intend to build a stylized Unity driving game featuring real-time procedural city generation, procedural cars, etc.

#### Inspiration/reference:
- Some of our reference projects include slowroads.io & the game easy delivery co.
- Our reference artwork (for style inspiration) is as follows: & our Pinterest board: https://pin.it/70blAtfEj 

| ![](https://i.pinimg.com/1200x/81/8c/7a/818c7ab620b90c0baac188f36f340555.jpg) | ![](https://i.pinimg.com/736x/2a/40/cc/2a40ccb6b418b46fdc386d659d0ab234.jpg) | ![](https://i.pinimg.com/1200x/2b/64/4e/2b644eac0a6301fad5ffb033d5666c2a.jpg) |
| :--: | :--: | :--: | 

#### Specification:
- The main features of our project is the procedural city with weirdness parameter, procedural cards, driving, post-process effects

#### Techniques:
- We will be using Unity & Houdini. 

#### Design:
- Simple free-body diagram illustrating how our program will fit together:

[![fbm-overview.png](https://i.postimg.cc/gc5gC4w3/fbm-overview.png)](https://postimg.cc/Rq71f7L0)

#### Timeline:
- Create a week-by-week set of milestones for each person in your group. Make sure you explicitly outline what each group member's duties will be.

# Milestone 1: 
## Alice: Procedural City Assets (building, benches, trees, sheep)
### Procedural Sheep



https://github.com/user-attachments/assets/9b8030da-bfa2-4cea-aa43-082639065629


### Procedural Benches

https://github.com/user-attachments/assets/a560f34a-9342-4538-aea1-65d383ff8e60


### Procedural Trees & Balcony
I followed this tree tutorial: https://www.sidefx.com/tutorials/procedural-stylized-trees-with-houdini-and-ue4/

<p float="left">
  <img src="readmeAssets//tree.png" width="400" />
  <img src="readmeAssets//balcony.png" width="400" /> 
</p>


## Jimin: Procedural City Assets (building, poles, lights)
### Lampposts and Poles
<img src="readmeAssets//streetlamp.png" width="600"/>
<img src="readmeAssets//modernlamp.png" width="600"/>

## Christopher: Procedural Car Skeleton
I researched car generators and did not really find any. Therefore, I planned out the overall car design myself and created a procedural skeleton for my car. 

<img src="readmeAssets//carSkeleton.png" width="600"/>

## Overall Progress:
We did not get as much done the first milestone as we hoped, as we spent a lot of time discussing ideas. Creating this number of procedural city assets proved to be more time consuming than expected. For the procedural car, it was hard to get started since there are not many resources online on procedural car generation. 

# Milestone 2:
## Alice: Putting city together
Finished procedural building not done in the last milestone:

### Procedural Building

https://github.com/user-attachments/assets/22030a01-3493-47fe-8915-ec30c992f34c

### Procedural City
I did the roads and varied the buildings. I had a much harder time than expected randomizing the buildings/windows, and this took a lot of time. I heavily used the "Labs Lot Subdivision" node. 
I used this city as a reference: https://www.artstation.com/artwork/kQ3wgn

<img src="readmeAssets//milestone2city3.png" width="600"/>

## Jimin: 
Finished procedural building and additional assets not done in the last milestone:

### Procedural Building 
<img src="readmeAssets//jiminBuilding.png" width="600"/>

## Christopher: Procedural Car Exterior
I built upon my car skeleton and created the exterior from some of the openings left by the skeleton. Creating the side faces from the edges proved to be harder than I though initially as I had to account for the change in the edge numbering due to changing some of the parameters such as the front/back windows and the rear door top parameters.   
<p float="left">
  <img src="readmeAssets//carExterior1.png" height="250" />
  <img src="readmeAssets//carExterior2.png" height="250" /> 
</p>

## Overall Progress:
We made relatively good progress for this milestone. While we did not fully put together the city at this point, we have all the individual assets done. The car is coming along. 

# Milestone 3 (Final):
## Alice: Polish up city + Unity 
When we tried to import the city into Unity, we realized that the city had way too many primitives (around 10 million). I had to reduce the city to around 150k primitives to get it to load into Unity. I added parks with trees and benches, reduced the polycount, and also had to remake all my materials into unity materials (which made them default grey in houdini). I did a lot of debugging. 

<img src="readmeAssets//milestone3city.png" width="800"/>

## Jimin: Polish up city + Unity + Houdini Engine
I added the sidewalks, which include two different types of lampposts and sheep. I imported the HDAs into Unity. I did a lot of debugging. Alice and I worked together to do the city chunking and driving in Unity. 

<img src="readmeAssets//cityunity.png" width="800"/>

## Christopher: Procedural Car Interior
I created the interior of the car, finishing the procedural car. 

<p float="left">
  <img src="readmeAssets//carInterior1.png" height="250" />
  <img src="readmeAssets//carInterior2.png" height="250" /> 
</p>

https://github.com/user-attachments/assets/909dd08e-9ba0-4b75-a788-5f73ed645652

# Overall Thoughts:
Our initial project scope was too large, and we spent a lot of time trying to fix HDA/Houdini Engine issues; getting our assets from Houdini to Unity took a lot more work than we expected. We did accomplish our main goal of creating a driving game with a procedurally generated city and cars. We created all the assets ourselves - but baking that many assets took an extremely long time. We unfortunately did not have enough time to make a weirdness parameter for our city. With more time, we definitely could have implemented that and polished up our game more. 
