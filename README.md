# Bixal Presentation Template

The purpose of this project is to enable Bixalers to create presentation content using a webpage instead of tools like Google Slides or PowerPoint.

**[View templates and example content](https://bixal.github.io/presentation-template/)**

Why would you want to do this? Here are a few reasons:

- Inherently more accessible and responsive
- Robust version control and collaboration tools with GitHub
- Better separation of content and presentation
- More open and shareable
- More fun

## Features

- Built on the U.S. Web Design System
- Includes common templates
    - Title
    - Subtitle
    - Blockquote
    - Text
    - Image with link
    - Text with image background
- Uses Bixal brand fonts and colors
    - Novel Pro and Proxima Nova typefaces
    - External CSS referencing [brand colors](https://cdn.jsdelivr.net/gh/bixal/brand-css@v2.1/style.css)
    - USWDS-style [utility classes](https://cdn.jsdelivr.net/gh/bixal/brand-css@v2.1/utilities-for-uswds.css) to apply brand colors to different elements
- Example slides
- Automatic slide count and next slide links
- Presenter notes available on the [`/notes/`](https://bixal.github.io/presentation-template/notes/) page of your site.

## How to

Navigate to the `_slides` folder to edit or add slides.

### Understand the code

Within the files, there are two distinct sections.

- **Front matter**: the text **between** a pair of dashes. This is where the majority of your slide styling occurs.
- **Content**: the text **underneath** the dashes. This is the main content, or "body", of your slide.

![Screencast of annotations on a code snippet distinguishing between its two main sections.](https://user-images.githubusercontent.com/52218695/134966615-38bce667-12f0-4bb3-b928-1928d32ffd1b.png)

### Add a title

- Titles can be added to the `title` term and will appear as top-level headings.
- Titles will not appear on the slides with the "blockquote" template, but it's best to have a title for consistency and traceability. 

### Change color

- You can apply color to the `text-color` and `background-color` terms by simply plugging in a color from Bixal's branding options:
  - orange
  - green
  - light-blue
  - teal
  - red
  - maroon
  - purple
  - navy

### Add images


If you're uploading an image, go to [/assets/img](/assets/img) in your repository and press the `Add file` button.

- Use the "text-with-image-bg" template if you're intending to use an image as a background image.
  - Add the image file name or image URL to the `bg-image` term.
- Use the "image-with-link" template if you're intending to set context with images and links. 
  - Add the image file name or image URL to the `image-source` term.
  - Make sure to include the appropriate image information to the `link` and `image-alt-text` terms!

#### Rearrange the text or image

- To change which side you want the text to be on, include the following term:
  - `text-order:` (first or last) 
- To change which part of an image you want to appear on the slide, include the following term:
  - `image-alignment:` (left or right)

### Add presenter notes

- Presenter notes can be added to the `notes` term and will only be seen by the presenter.
- They can be accessed through the `/notes/` page of your site (i.e. bixal.github.io/presentation-template/notes/)

### Order your slides

How you name your slides will determine the order they will appear.

- Your files will automatically be sorted alphabetically.
- You can control the order by adding numeric values to the front of your slide's file name (i.e. 1, 1.1, 1.2, 2, 2.4, 3, etc.). 
- The lowest value will appear first and the highest value will appear last.
