## For the use of data for [Data Art Symposium](https://data-art.info/)

1. Artwork Images: [Available on Kaggle here](https://www.kaggle.com/datasets/yangyuwang/wikiart-images)

Please download it from kaggle manually or by the code below in bash.

```bash
kaggle datasets download -d yangyuwang/wikiart-images -p /content/artworks/
unzip /content/artworks/wikiart-images.zip -d /content/artworks/
```

2. Artwork Info: [artwork_data_merged](artwork_data/artwork_data_merged.csv)

To link the dataset to images, please use the column of `image_n` in the csv file and the `caption` key value in json files on Kaggle.

3. Artist Description:

See [artist_desc](artist_data/artist_desc.json). If you want to use the raw data, please see [demographic_information](artist_data/demographic_information.json).

In both json file, the key are the artist url names. (It is not necessary the lower case with hyphen linkage of the real names, but most cases are in this format. For example, Vincent van Gogh is vincent-van-gogh.)

To link the description and demographic information to artworks, please use the column of `Artist_name`. For some data scraping issues, some artist names are added a "en/". Remember to remove those at the first place.


