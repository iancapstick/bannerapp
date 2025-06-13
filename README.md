# Banner Creation Tool

A free, interactive web tool that helps activists and organizers create effective protest banners based on their specific needs, budget, and available resources.

## Purpose

This tool guides users through a series of questions to generate personalized recommendations for creating protest banners, including:
- Exact dimensions and specifications
- Shopping lists with budget-appropriate materials
- Step-by-step creation methods
- Professional tips organized by category

## Live Tool

Access the tool at: [https://iancapstick.github.io/bannerapp/banner-tool.html](https://iancapstick.github.io/bannerapp/banner-tool.html)

## Features

- **Personalized Recommendations**: Based on 8 key factors including budget, skills, timeline, and weather conditions
- **Smart Sizing**: Automatically calculates banner dimensions, font sizes, and visibility distances
- **Material Lists**: Budget-appropriate shopping lists with specific product recommendations
- **Organized Tips**: Professional advice categorized into Lettering, Construction, Weatherproofing, and Finishing
- **Multiple Export Options**: Print, save as text, copy to clipboard, or email results
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Embeddable**: Can be embedded in other websites using an iframe

## Embedding the Tool

To embed this tool in your website, use:

```html
<iframe 
    id="banner-tool-iframe"
    src="https://iancapstick.github.io/bannerapp/banner-tool.html" 
    width="100%" 
    height="800" 
    frameborder="0" 
    style="border: none; min-height: 800px;">
</iframe>

<script>
window.addEventListener('message', function(e) {
    if (e.origin !== 'https://iancapstick.github.io') return;
    if (e.data && e.data.type === 'bannerToolHeight') {
        const iframe = document.getElementById('banner-tool-iframe');
        if (iframe) {
            iframe.style.height = (e.data.height + 20) + 'px';
        }
    }
});
</script>

## Contributing
Feedback and contributions are welcome! Please open an issue or submit a pull request.

License
This tool is free to use and modify. Created to support activists and community organizers worldwide.

Acknowledgments
Special thanks to our beta testers whose valuable feedback helped shape this tool into what it is today.
