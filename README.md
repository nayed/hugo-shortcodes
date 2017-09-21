# Hugo-Shortcodes
Those are shortcodes I created for [Hugo](https://gohugo.io/).

### Install
Inside your Hugo project create a `layouts` folder if it does not exist and clone:
```
$ git clone https://github.com/nayed/hugo-shortcodes.git layouts/shortcodes
$ rm -rf layouts/shortcodes/.git layouts/shortcodes/README.md
```
You have to delete .git and README.md otherwise Hugo will output error message when parsing `layouts/shortcodes`.

Or you can copy .html file and put them in yout layouts/shortcodes folder.

### Included:

#### Google Maps `google-maps.html`:
In your `config.toml` file add in the Params section your Google Maps Embed API key:
```toml
[Params]
googleMapsEmbedAPIKey="YOUR_API_KEY"
```

You are now ready to embed a map in your article:
```
{{< google-maps height="500" width="800" lat="45.757175" lng="4.831332" zoom="5" >}}
```

Will ouput:

![](https://i.imgur.com/FN330NI.png)

