<h1 align="center"> ImgPile API </h1>

## **Description**
> `imgpile` is a custom api written in python that scraps image data from [imgpile.com](https://imgpile.com/). </br> It takes an album's `url` and returns every image's details as `json` data.

## **Usage**
1. Install [Python 3.x](https://www.python.org/download)
2. __Download__ or __clone__ this repository on your local machine.
3. Extract the `zip` file.
4. Open terminal in this folder and run `pip install -r requirements.txt`
5. `import` this api in your script.

## **API Methods**
> There are several methods in this api but they are used by the api itself for specific tasks. You can use `get` method which does all the work automatically. </br>

`get(url)`
> This method takes `url` input which must be the url of an album from [imgpile.com](https://imgpile.com/) and returns a list of dictionaries. each dictionary is the data of an image.


`Reponse Format & Keys`
``` json
[
    {
        "image_url": "URL of image.extension",
        "image_link": "Link to the image",
        "thumb_url": "URL of thumbnail.extension",
        "lq_url": "URL of low-quality image.extension",
        "title": "Image title",
        "size": "32.2 MB",
        "resolution": "5232 x 7845",
        "image_type": "JPG",
        "views": "View count of this image",
        "likes": "Like count of this image",
        "uploader": "Name of uploader of this image",
        "uploaded": "1 year ago"
    },
    {
        ...
    },
    {
        ...
    }
]
```
