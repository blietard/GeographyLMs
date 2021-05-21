# GEOGRAPHICAL RELATIONS WITH LANGUAGE MODELS

Are there any meaningful relations in LMs vector representations of geographical nouns (cities/countries/etc) that correspond to real-life spatial relations between entities ? 

## Useful links :
https://www.dropbox.com/s/mqux75f5cu0ndav/bert2maps.zip
https://www.sbert.net/docs/pretrained_models.html
 

## Ideas
* Compare pairs of real Life (RL) distance / vector similarity (VS) between 2 points (Anders’s code)
* **Display in 2D** such pairs (x: RL dist / y: VS)
* Compare relations of **closeness/far distance** between two points
    - Nlp context : 
      - Direct relation : “A is close from B”
      - Indirect relation : “He drives from A to B” 
    - Compute RL distance between A and B
    - Compute VS between A and B contextual representations
          *(to get word embeddings, maybe use INRIA’s mangoes pckg)*
* **Cardinal relations** ? North, South, etc.  
  - “Fact checking” ?? “A is in North Hemisphere” and compare sentence embeddings when it is **true or false** // also possible with “A is north of B” for each pair of points
  - With simple context “my favorite city[/country] is”, compare VS between 2 points according to their **relative cardinal position**.
      *“If A is north of B, we observe a shift in vector” or smthg like that ???*
