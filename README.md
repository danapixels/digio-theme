# Digio theme
### A pixel, ASCII, minimal, retro theme for [Hugo](https://gohugo.io/).

#### Home page
![screenshot](https://raw.githubusercontent.com/danapixels/digio-theme/main/images/screenshot.png)

### Sections
![sections](https://raw.githubusercontent.com/danapixels/digio-theme/main/images/digio-section.png)

### Posts
![post](https://raw.githubusercontent.com/danapixels/digio-theme/main/images/digio-page.png)

## Demo site
To see how this theme works, view my current [blog](https://danablog.dev).

## Features
- Tagging
- External links can be added as a part of post lists (sorted by date along with posts)
- Mobile-friendly
- Switch between icons to indicate different posts

# Installing Hugo (extended)
To use `digio-theme` you need to install Hugo Extended by following [https://gohugo.io/getting-started/installing/](https://gohugo.io/getting-started/installing/).


# Installing Tailwind

```
# Install Tailwind
npm install tailwind postcss autoprefixer

# Useful script for later will compile tailwind into CSS once, good for production
npm run build

# Useful script for later will continuously compile tailwind into CSS, good for development
npm run watch
```
*The scripts referenced were taken from this video from the [Hugo Conference](https://www.youtube.com/watch?v=0WJ2lWNhqm8).*

# Create a site and cd into it
```
hugo new site <your website's name>
cd <your website's name>
```

# Clone theme into your themes folder
```
mkdir themes
cd themes
git clone https://github.com/danapixels/digio-theme
```

# Run the server locally
```
hugo server -d
```

# Open the site in your browser
```
open http://localhost:1313/
```

# Customization
These can be found in the theme's folder. 
*Note: To keep theme images, you will need to copy the theme's static folder to your static folder (it may not copy them automatically).*


## Home page front matter
Located in `_index.md` in the `content` folder.
```
# Change the home profile picture
portraitImage = "/yourimage.png"

# Change the bolded intro title
introTitle = "Introduce yourself here!"

# Change the summary of the homepage
introBody = "Give the audience a little summary/introduction about what to expect in this ASCII, black and white, pixel focused theme."

# Change the status image
statusImage = "/status.png"

# Change the status text
statusText = "A way to let everyone know what you're up to..."

# Change the currently watching image
watchingImage = "/watching.png"

# Change the watching text
watchingText = "How to create a Hugo theme from scratch — Berkay Çubuk // HugoConf 2023"

# Change the video URL
watchingUrl = "https://www.youtube.com/watch?v=0WJ2lWNhqm8"
```

## About me front matter
Located in `me.md` in the `content` folder.
```
# Change listed likes
likes = [
  "Example 1",
  "Example 2",
  "Example 3",
  "Example 4",
  "Example 5",
  "Example 6",
  "Example 7",
  "Example 8",
  "Example 9",
  "Example 10",
]

# Change listed dislikes
dislikes = [
  "Example 1",
  "Example 2",
  "Example 3",
  "Example 4",
  "Example 5",
  "Example 6",
]

# Change listed hobbies
hobbies = [
  "Example 1",
  "Example 2",
  "Example 3",
  "Example 4",
  "Example 5",
  "Example 6",
]
```

## Set the post and section icons that will be shown
```
# Heart icon
icon = "/contribute.png" 

# Book icon
icon = "/writing.png"
```

## Posts front matter
```
# Make your own or choose `contribute.png` for a heart or `writing.png` for a book.
listIcon = "/writing.png"

# This will show in your sections and your homepage.
teaser = "Some flavor text here..."
```

## Sections front matter
```
# This will treat your external link as a post and be organized according to the date you set. 
externalLinks = [
  { title = "external example", url = "https://gohugo.io/", date = "2025-04-17", icon = "/contribute.png", teaser = "Teaser for your external link" },
]
```

## License
[GNU General Public License 3.0](https://www.gnu.org/licenses/gpl-3.0.en.html)
