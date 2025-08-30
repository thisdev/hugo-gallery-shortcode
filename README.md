# Hugo Simple Gallery Shortcode

A lightweight, responsive image gallery shortcode for Hugo with integrated lightbox functionality. No external dependencies required.

## Features
- Responsive grid layout (2-5 images per row)
- Support for multiple galleries on one page
- Stacked image gallery as a second layout option
- Supports different file types (.jpg, jpeg, .png, .gif, .webp)
- Built-in lightbox
- Keyboard navigation (←, →, ESC)
- No external dependencies
- Hover effect
- Simple installation
- Light/Dark mode support

## Click screenshots for a live demo

### Screenshot 1: Image gallery
[![hugo-gallery-shortcode-example](https://github.com/user-attachments/assets/9cd81f33-33f0-4883-9665-d15eb88580bf)](https://blog.bitlager.de/posts/tech/hugo-gallery-shortcode-example/)

### Screenshot 2: Stacked image gallery
[![hugo-gallery-shortcode-example](https://github.com/user-attachments/assets/57e1dd51-fe59-48db-8d69-35893f545845)](https://blog.bitlager.de/posts/tech/hugo-gallery-shortcode-example/)

## Installation
1. Create a `shortcodes` directory in your Hugo project's `layouts` folder if it doesn't exist:
2. Copy `image-gallery.html` and/or `stacked-image-gallery.html` into the `layouts/shortcodes` directory

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
## My article

### First gallery
{{< image-gallery gallery_dir="/images/my-gallery1" >}}

### Second gallery
{{< image-gallery gallery_dir="/images/my-gallery2" >}}

### Stacked gallery
{{< stacked-image-gallery gallery_dir="/images/my-gallery2" >}}
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
