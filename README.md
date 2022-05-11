# Horiseon Social Solutions

## Service that helps businesses grow and develop from the web and social media.

This website functions as an easy way for businesses to see the services that Horiseon provides, which are all related to the growth and development of social media accounts and websites.

The three large blocks of text outline the ways in which Horiseon could help the customer, which are Search Engine Optimization, Online Reputation Management, and Social Media Marketing. The header navigation box is linked to these three items. The sidebar details the benefits of using these three methods, including Lead Generation, Brand Awareness, and Cost Management.

## Changes

### Front End

There wasn't much accessibility at first.  To fix this, I inserted < alt > tags on the images and pictures.  This functions to make it easier for screen readers or those with disabilities to use and interact with the website as well.  It also will tell any user what the image if for some reason it is unable to load.

There was also a title missing in the browser tab, so I gave it a short description of the purpose of the comapny. 

### Back End - HTML

I cleaned up the code in a number of ways. 

The first is including semantic html instead of the more vague elements originally used.  This would include items such as turning the < section > with the header and navigation to the more specific < header > so that the browser can more easily read the code. It also helps to connect the .css file as it is clear what is connected to what.  The same was done to the < footer > sections

I also turned the < div > containers that had the main content of the website into 3 individual < article > tags.  They are related but each have independent content and images, so it makes sense to clarify their functions. This also negates the need for so many identifiers, so I deleted the extra class selector in the individual < article >.

The < div > containers for the sidebar content stayed the same since there seemed all to be listing the benefits of the service, but the entire < section > was changed to an < aside > tag to inform the next coder that these items are included in the sidebar. It also distinguishes this section from the other < section > tags/selector on the page and in .css.

I also added comments to make it easy to distinguish the different sections.

### Back End - CSS

I started by changing the selectors to match the new semantic HTML.  This made it easier to know what exactly was connected. For exmaple, the entire < aside > section now refers to just that section tag, along with the clarifying selectors within it. Sections for the hero and the main content must use a class selector since their tags are more general. The < header > and < footer > selectors were also updated.

The next time I changed was the order of the code.  Some sections were jumbled in the sense that multiple sections were being referred to, but not in chunks.  I rearranged it so the styles of one section are all together (i.e. all the < footer > styles are in the same part of the code, uninterrupted). After this, I made comments to clarify what section is which so that the next coder can easily read the file.

## Lesson

The main thing to learn from this challenge is that accessibility is very important in both front and back ends of web development.  First, semantic HTML makes it easier to both read and edit the code for both HTML and CSS. Once a page gets more complicated, there are multiple sections with the same tag, so if one is able to be specified, the browser (and other coders) can read the stylized code easier.  

Second, disorganized code in the .css styling sheet makes it harder for future coders to work on a project, so it is better to always try to comment and keep it in order.  If there's ever a contradiction, CSS will implement the code written later in the program, so its important to keep track of what you are styling so nothing gets overridden. 

In terms of user experience, there were no < alt > tags on the images, which make the page inaccessible for anyone using a screenreader. This opens up the client to litigation, which is not what you want. It also lets viewers having technical or web issues see a written description of what they're supposed to be seeing. 




