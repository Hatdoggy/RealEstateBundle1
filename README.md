Hello this is the simplified guide into using the website template you have just purchased! Please follow this step by step process to smoothly use your new website. Thank you again and all the best wishes for you.

====================================================================================================

Apex Estates Premium Real Estate Template Bundle Easy Setup & Customization Guide

Welcome to your new premium real estate website templates! This guide will help you easily change the text, swap out photos, update house floor plans, connect your contact forms, and launch your websites online—no coding experience required.

====================================================================================================

    Finding Your Files

When you open your template folder, you will see the following layout:

    HTML/ – Contains the actual website files and components.
        single-property.html (Single Luxury Estate Page)
        broker-funnel.html (Solo Agent Brand Funnel)
        pre-construction.html (Condo Developer Landing Page)
        components/ (Reusable template blocks)
    User_Guide/ – Contains this documentation and customization guide.
    screenshots/ – Contains high-resolution visual screenshots of the websites.
    Licensing.txt – Credits and attribution details for fonts, scripts, and images.

====================================================================================================

💡 How to edit these files: Right-click on any of the .html files and select Open With, then choose a simple text program like Notepad (Windows) or TextEdit (Mac). Better yet, download a free tool like VS Code for an easier viewing experience.

    Changing Text, Headlines, and Property Specs

To change any text on the website, open the file in your text editor, press Ctrl + F (Windows) or Cmd + F (Mac) to open the search bar, type the text you want to change, and type over it. Changing Main Headlines

Search for the default name of the villa, like VILLA SOLIS. Just delete that name and type your new property name (e.g., THE CLIFFSIDE RESIDENCE) right in its place. Changing Property Specs (Square Footage, Beds, Baths)

Search for numbers like 11,250 SQ. FT.. Swap out that number with your property’s actual size. Be careful not to delete any of the surrounding code brackets (< or >).

====================================================================================================

    Swapping the Logo, Photos, and Backgrounds

All images and logos on your website are loaded using code tags that look like this: src="image-path-or-link". You can personalize any image on the site simply by changing this src value to point to your own files or online URLs.

Updating the Brand Logo The templates use two logo files located in the assets/ folder: logo-light.svg (for dark backgrounds) and logo-dark.svg (for light backgrounds).

    To change the logo, you can overwrite these files directly in the folder with your own logo images.
    Alternatively, you can open the HTML files and change the src attribute directly: search for id="header-logo" and replace the src="..." value (e.g., src="assets/logo-light.svg") with the path to your new logo file.
    Scroll Note for Single Property: In single-property.html, the logo automatically swaps when scrolling down to maintain contrast. If you use new file names for your logo images, make sure to also update the file names in the // HEADER SCROLL TRANSITION script section at the bottom of the HTML file.

Replacing Photos and Backgrounds

    Find the image tag by searching for the section it belongs to (e.g., the living room).
    Look for the web link inside the quotes, which usually looks like: src="https://images.unsplash.com/..."
    Delete that link and replace it with either a new web link to your photo, or a relative file path to a photo on your computer (e.g., assets/images/living-room.jpg).

📐 Photo Tips for a Beautiful Website:

    Big Background Images: Use sharp, high-quality, wide landscape photos. Try to keep the file size small so your website loads instantly.
    Gallery/Grid Images: Use tall, vertical photos (like portrait mode on your phone) to keep the layout looking like an elegant magazine.

====================================================================================================

    Editing Floor Plans and Blueprints

The interactive floor plans use clean layout shapes called SVGs. You don't need to be a designer to change the labels on them. Changing Room Labels

Open the file, search for a room name (like LIVING & GALLERY). Simply delete those words and type your new room name (like GUEST SUITE). Using a Completely New Floor Plan

If your architect gave you a custom floor plan image file ending in .svg:

    Open your new floor plan file in Notepad.

    Copy all the text inside it.

    Find the old section in your website template and paste your new code right over it.

====================================================================================================

    Setting Up Forms and Pricing Sliders Connecting Forms to Your Email or CRM

By default, when someone clicks "Submit" on a form, a simple popup box appears on the screen. To actually receive these messages in your email or link them to a CRM system (like GoHighLevel or Zapier):

    Search for id="inquiry-form".

    Look for action="https://your-backend-api.com/submit".

    Replace that placeholder link with the custom webhook or form submission link provided by your CRM tool.

Adjusting the Property Size Slider

On the broker website, clients can slide a bar to choose a house size. You can adjust the limits of this slider easily:

    Search for id="slider-size".

    Change min="1000" to your lowest desired size (e.g., 500 sq. ft.).

    Change max="15000" to your highest desired size (e.g., 20000 sq. ft.).

    Change value="3500" to set where the slider handle sits when the page first loads.

====================================================================================================

    Adding Calendar Tools (Calendly or GoHighLevel)

If you want to replace a standard contact form with an interactive booking calendar so clients can schedule appointments directly:

    Copy the "Embed Code" or "iframe link" provided by your calendar software (Calendly, GoHighLevel, etc.).

    In your website file, search for the contact form block (it starts with
    and ends with ).

    Delete that entire form block and paste your calendar embed code right in its place.

====================================================================================================

    Uploading/Importing into Website Builders & CMS

These templates are standard HTML5/CSS3/JavaScript files. This means you can easily import them into your favorite website builders, funnel systems, or Content Management Systems (CMS).

📥 GoHighLevel (GHL) / Funnel Builders

    Log in to your GHL account, go to Sites -> Funnels or Websites, and create a new page.
    Add an HTML/JS element to your page layout.
    Open your template HTML file, copy all the code, and paste it into the HTML/JS editor.
    Upload any assets (like your logo and custom images) to the GHL Media Library, copy their URLs, and update the src links in your code.

WordPress

    Using Gutenberg (Block Editor): Add a Custom HTML block to your page and paste the template code.
    Using Elementor/Divi/Page Builders: Insert an HTML widget/module into the layout and paste the code.
    As a Standalone Landing Page: You can upload the template files directly to your web server using FTP or a File Manager in your hosting control panel (under public_html).
    Make sure to update the image links (src) in the code to point to your media library URLs (e.g., https://yourwebsite.com/wp-content/uploads/your-image.jpg).

Shopify

    Go to your Online Store -> Themes, click the three dots next to your theme, and select Edit Code.
    In the template files or sections, you can create a new section, add a Custom Liquid or HTML block, and paste the code.
    Upload your images to Shopify Content -> Files, copy their links, and paste them into the src="..." tags.

Squarespace & Wix

    Add an Embed or Code Block to your section.
    Select the HTML setting, paste the template code, and save.
    Ensure all image links (src) point to external URLs where your pictures are hosted (such as Wix's media manager link or an external hosting service).

====================================================================================================

    Adjusting, Resizing, and Styling Images

To make the design match your listing perfectly, you can adjust how the images display on screen directly in the HTML code using Tailwind CSS classes.

Replacing Image URLs

    In your code editor, locate the <img> tag you want to edit.
    Replace the link inside src="..." with your own image link:
        For local files: src="assets/your-photo.jpg"
        For web links: src="https://yourdomain.com/photo.jpg"

Adjusting Image Sizes You can control the width (w-) and height (h-) of any image by modifying the Tailwind classes in the class list:

    Full Width: Use w-full to make an image fill its container.
    Specific Widths: Use w-32 (8rem/128px), w-64 (16rem/256px), etc.
    Height limits: Use h-48, h-64, h-96 (24rem/384px) or h-screen (full viewport height) to control the vertical space an image occupies.
    Aspect Ratios: Control the shape using aspect-video (16:9), aspect-square (1:1), or aspect-[4/3].
    Fit Behavior: Use object-cover to make the image fill the frame without stretching (highly recommended), or object-contain to fit the entire image inside the frame.

Adding Rounded Corners & Shadows

    Rounded Corners: Add rounded-lg, rounded-xl, or rounded-full (for circular profile images) to the class="..." list.
    Subtle Shadows: Add shadow-sm, shadow-md, or shadow-lg to make images pop out from the background.

====================================================================================================

    Launching Your Website Online (100% Free)

Because these templates are self-contained and highly optimized, you do not need to pay for expensive web hosting. Here is the easiest way to launch your site:

The Drag-and-Drop Method (Netlify)

    Go to Netlify.com and create a free account.
    Click on the Sites tab in your dashboard.
    Scroll down to the box that says "Drag and drop your site folder here".
    Drag your entire project folder from your computer and drop it into that box.
    You're live! Netlify will instantly give you a link to view your live website. You can also hook up a custom domain name (like yourdomain.com) for free inside their settings tab.
