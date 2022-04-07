# 2022-04-07
## Building a web frontend for exploring featured images, their labels and colors

The plan is to have a frontend where you can filter all photographs that are featured images (<10000 images) by labels and colors.
To facilitate not having to send to heavy a dataset to the browser, colors should be reduced to an 8-bit value. This will also make it easy to filter by similar, not neccesary identical colors.





# What i have

Following datasets:

- URLs of all [featured images on Wikimedia commons](https://commons.wikimedia.org/wiki/Commons:Featured_pictures/)
- for all pics, information on how many views per month it has gotten since it was uploaded
- for all pics, information on whether it is a photograph (has camera metadata) or not
- for all pics that are photographs by the above definition, i have Google Vision label recognition data
- for all the photographs i have also performed cluster analysis to determine the most prominent colors in the pic

# What i want to find out

- What tags correlate most strongly with views per month, positively or negatively, for all the photographs that are featured pictures
- What approximate colors correlate most strongly with views per month, positively or negatively, for all the photographs that are featured pictures
- which tags cluster a lot / are more often seen together than expected by chance, or the reverse

