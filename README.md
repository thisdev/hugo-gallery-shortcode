# Hugo Simple Gallery Shortcode

A lightweight, responsive image gallery shortcode for Hugo with integrated lightbox functionality. No external dependencies required.

## Features
- Responsive grid layout (2-5 images per row)
- Supports different file types (.jpg, jpeg, .png, .gif, .webp)
- Built-in lightbox
- Keyboard navigation (←, →, ESC)
- No external dependencies
- Hover effect
- Simple installation
- Light/Dark mode support

## Screenshot (click for a live demo)
[![hugo-gallery-shortcode-example](https://github.com/user-attachments/assets/2216d8f6-f6c8-462f-bd79-5c8c8905a2ae)](https://blog.bitlager.de/posts/tech/hugo-gallery-shortcode-example/)

## Installation
1. Create a `shortcodes` directory in your Hugo project's `layouts` folder if it doesn't exist:
2. Copy `image-gallery.html` into the `layouts/shortcodes` directory

## Usage

1. Place your images in any directory you want, e.g.:
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

## Future Features
This gallery shortcode is under active development. The following features are planned for future releases:

### Planned Enhancements
- [x] Check for file types (.jpg, jpeg, .png, .gif, .webp)
- [x] Custom image captions in lightbox view
- [ ] Vertical gallery layout option (images stacked)
- [ ] Configurable grid layout (adjust number of images per row)
- [ ] More gallery customization options
- [ ] Separated files (CSS/JS)
    - `gallery.css` for styling
    - `gallery.js` for lightbox functionality
    - `image-gallery.html` for structure
- [ ] Markdown-style image syntax support

### Want to Contribute?
Feel free to:
- Open issues for bug reports or feature requests
- Submit pull requests for improvements
- Share your ideas in the discussions

Your contributions to make this gallery shortcode even better are welcome!

## License
MIT

## Credits
Based on the idea from [hugocodex.org](https://hugocodex.org/add-ons/image-gallery/)  
Inspired by [nicokaiser - hugo theme gallery](https://github.com/nicokaiser/hugo-theme-gallery)
