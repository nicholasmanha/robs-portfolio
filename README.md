# Robert's Portfolio Documentation
Portfolio for Robert Burke's films and productions. Built using React.
## MovieListing
MovieListings arethe basic component for displaying work you've done. They involve a thumbnail of the media, a description of the media, and more. They are dynamic with the information given.
### Example 1
*this example uses a video for the thumbnail*
```
    <MovieListing
            title="Title of the media"
            url="link_to_the_media"
            readmore="Stuff you did for this media would go here."
          >
            The description of the media would go here. <br/>
    </MovieListing>
```

### Example 2
*this example uses an image for the thumbnail*
```
    <MovieListing
            title="Title of the media"
            image="link_to_the_image"
            tagline="Tagline for the media would go here."
            link={[
              "Link Title",
              "https://link_url.com",
            ]}
          >
            The description of the media would go here. <br/>
    </MovieListing>
```

> Note how the second example doesn't even have a "readmore" attribute. This is because you can ignore attributes that you won't be using in that particular Movielisting.

### Attributes
* `title` The title of the media | string, array
* `url` The link to the media | string
* `image` The link to the image | string
* `tagline` The tagline of the media | string
* `readmore` What you did for the media | string
* `link` Any external links for the media | array
* `children` The description of the media | string
## FAQ
### What files should I be touching?
The only files you would want to be editing is the Experience.jsx file and MAYBE the Home.jsx file. They are in src > pages.
### How do I make a styled title? 
Use an array with html in the element
* Example: `title={["In the Middle", <small> - Coming Soon</small>]}`
> Always use {} around an array.
### How do I use the `link` attribute?
This too is an array. The first element of the array is the display text, the second element is the url. 
* Example: `link={["Link Title", "link_url.com"]}`
### My video isn't working on the website!
This is commonly because you are not using the embeded link for the video. Go to your video, click "share" and then embed, and copy the url in the code given.
