# Responsive Design

Today, many people view websites on devices other than computers, such as smartphones and tablets. It’s important to make sure your website is readable to people on all devices.
- One way we can achieve this is through knowledge of the viewport. The viewport is the part of the screen that is actually visible to the user at any given time. By default, many webpages assume that the viewport is the same on any device, which is what leads to many sites (especially older ones) being difficult to interact with on mobile devices.
- One simple way to improve the appearance of a site on a mobile device is to add the following line in the head of our HTML files. This line tells the mobile device to use a viewport that is the same width as that of the device you’re using rather than a much larger one.
<meta name="viewport" content="width=device-width, initial-scale=1.0">
- Another way we can deal with different devices is through media queries. Media queries are ways of changing the style of a page based on how the page is being viewed.
- For an example of a media query, let’s try to simply change the color of the screen when it shrinks down to a certain size. We signal a media query by typing @media followed by the type of query in parentheses:

            @media (min-width: 600px) {
                body {
                    background-color: red;
                }
            }

            @media (max-width: 599px) {
                body {
                    background-color: blue;
                }
            }


####  infintie scroll


window.onscroll = () => {
    if (window.innerHeight + window.scrollY >= document.body.offsetHeight) {
        load();
    }
};

