# Homework 1
## Description
The goal of this homework assignment was refactor provided HTML to make it more accessible and readable using semantic HTML. 

## HTML changes made
* Replaced nearly all <div> tags with semantic elements, like <header>, <nav>, <main>, <aside>, <section>, and <footer>. 

* Renamed the <title> of the website to "Horiseon: Social Solution Services" to be more descriptive. 

* Added descriptive alt attributes for all images on the page. 

* The Search Engine Optimization link was nonfunctional - the <a> tag for this link in HTML was missing an ID tag like the other nav links, so the necessary ID tag was added.

* Some classes were changed per the CSS changes described below.

## CSS changes made
* Refactoring the <div> containing the navigation links to <nav> broke the CSS .header selector - refactored it to be .header nav instead of .header div. 

* Many selectors are repetitive and assign the same formatting to elements - collapsed these and reassigned classes to elements with the same formatting:
    * Replaced all the .benefit- selectors with .aside-style and all of the .benefit- images with .aside-style img
    * Replaced all the individual h3 selectors with a broad h3 selector
    * Created a .content-style selector for search-engine-optimization, online-reputation-management, and social-media-marketing, as they were repetitively formatted
    * All of the images in the main body are formatted the same, so replaced the individual image selectors with a broad img selector (images in the benefits/aside section are more specifically formatted using their class tag)
    * Created a broad h2 selector to replace each individualized h2 

* Commented out each change described above with reasoning behind the change.

* Reorganized style.css so that the selectors are in order of appearance in index.html. 

## Remaining issues
* Line 27 - unsure of how to restructure the main image on the page because the image resides in CSS. Was not able to get it to behave correctly when moving it over to HTML and trying to format it as an img in CSS. 
    
* This image can't be assigned an alt attribute if it isn't an img element in HTML. Without an alt attribute, a major piece of content on the page is both not accessible via screen readers and lacks semantic HTML elements. 