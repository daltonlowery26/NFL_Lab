# Structure

## General Thoughts

- target var should be delta x or delta y
- if we make high quality embeddings can we just predict what the average player would do then add there unqiue embedding value
- this is a sequence to sequence problem
- most important feature to predict next postion is prior postion
- for the target var the most effiective choice is change in (x,y) from ground truth

## embed

- first step is an encoder that takes player prior and encodes that as a vector
  - replacement level, what does the average player do. encode this as the origin or as its own unqiue vector
  - encode based on what is optimal for predicting the next frame
  - do we create unqiue encodings for a given position
  
- qb embedding as part of the context embedding