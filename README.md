# Hugo Simple Gallery Shortcode

A lightweight, responsive image gallery shortcode for Hugo with integrated lightbox functionality. No external dependencies required.

## Features
- Responsive grid layout (3 images per row)
- Built-in lightbox
- Keyboard navigation (←, →, ESC)
- No external dependencies
- Simple installation
- Light/Dark mode support

## Installation
1. Create a `shortcodes` directory in your Hugo project's `layouts` folder if it doesn't exist:
2. Copy `image-gallery.html` into the `layouts/shortcodes` directory

## Usage

1. Place your images in a directory within your `static` folder, e.g.:
```
static/
└── images/
    └── my-gallery/
        ├── image1.jpg
        ├── image2.jpg
        └── image3.jpg
```

2. Use the shortcode in your markdown files:
```markdown
{{< image-gallery gallery_dir="/images/my-gallery" >}}
```

## Navigation
- Click on any image to open the lightbox
- Use arrow keys (← →) to navigate between images
- Press ESC or click the X to close the lightbox
- Click outside the image to close the lightbox

## Customization
The gallery uses CSS Grid for layout and comes with default styling. You can customize the appearance by modifying the CSS in the shortcode file.

## Compatibility
Tested with:
- Hugo Extended Version
- PaperMod Theme
- Other Hugo themes should work as well

## License
MIT

## Credits
Based on the idea from [hugocodex.org](https://hugocodex.org/add-ons/image-gallery/)
