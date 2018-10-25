# Icons API Integration
## Overview
The big idea behind the icons API is the ease of manipulation with visual content. Having just a huge bunch of icons files may not necessarily help you to efficiently and competitively produce and support agile development. Wouldn't it be much more better to have a dedicated platform like [Icons8](https://icons8.com/) that would cope with all sort of the challenges associated with managing, updating, and delivering the visual content in most suitable forms to outperform expectations of even the most demanding developers and UX designers? That is actually what the icons/photos services are all about. 

This is us, the Icons8, who takes the responsibility to maintain the whole [infrastructure](https://api.icons8.com/) of managing and accessing visual content to let our clients to focus on delivering new products to the market with highest pace and lowest cost possible.

In a nutshell, [icons API](https://api.icons8.com/) represents by itself a web service with a list of web methods to manipulate with the visual content on the fly. The web methods could be invoked from various types of applications either web, desktop, or mobile. This is how integration is being achieved. Such architecture gives a unique level of flexibility to our clients to develop very sophisticated applications with outstanding UX and optimised time-to-market.

## API functions

[Icons API](https://api.icons8.com/) handles requests from clients apps and returns both Base64-encoded icons and the meta information. Some of the operations are:
-   Searching for a string
-   Getting the categories
-   Getting the icons from a category
-   Searches for similar icons (icons that have similar tags)
-   Suggestions for find-as-you-type, etc.
-   Searching for a string
-   Getting the categories
-   Getting the icons from a category
-   Searches for similar icons (icons that have similar tags)
-   Suggestions for find-as-you-type, etc. 

Below is a complete list of operations with definitions and links to live test page:

| Operation | Definition | Live Test |
|:--|:--|:--:|
| [GET /api/iconsets/icon](https://api.icons8.com/manual/icon)|Returns several icons | [Try](https://api.icons8.com/try/icon)  |
|[GET /api/iconsets/icons](https://api.icons8.com/manual/icons)|Returns all icons in alphabetical order|[Try](https://api.icons8.com/try/icons)|
|[GET /api/iconsets/search](https://api.icons8.com/manual/search)|Returns icons by the specified search criteria|[Try](https://api.icons8.com/try/search)|
|[GET /api/iconsets/latest](https://api.icons8.com/manual/latest)|Returns several icons sorted by date, with the newest first|[Try](https://api.icons8.com/try/latest)|
|[GET /api/iconsets/similar](https://api.icons8.com/manual/similar)|Returns icons that similar to the given one|[Try](https://api.icons8.com/try/similar)|
|[GET /api/iconsets/total](https://api.icons8.com/manual/total)|Returns the total number of icons for different platforms|[Try](https://api.icons8.com/try/total)|
|[GET /api/iconsets/list](https://api.icons8.com/manual/list)|Returns lists with information about icons|[Try](https://api.icons8.com/try/list)|
|[GET /api/iconsets/categories](https://api.icons8.com/manual/categories)|Returns lists of categories|[Try](https://api.icons8.com/try/categories)|
|[GET /api/iconsets/category](https://api.icons8.com/manual/category)|Returns lists of icons in particular category|[Try](https://api.icons8.com/try/category)|
|[GET /api/iconsets/suggest](https://api.icons8.com/manual/suggest)|Returns suggests about icons and tags for given string|[Try](https://api.icons8.com/try/suggest)|
|[GET /api/iconsets/svg-symbol](https://api.icons8.com/manual/svg-symbol)|Returns SVG `symbol` image consists of specified icons|[Try](https://api.icons8.com/try/svg-symbol)|
|[GET /api/iconsets/download](https://api.icons8.com/manual/download)|Download icon's image|[Try](https://api.icons8.com/try/download)|

## Elements, Attributes, Parameters

## API vs. JSON (pros&cons)
### What If We Go out of Business etc.
## Examples

## Use cases
These are examples of API usage in production applications:

-   **Template customisation.**  This is how  [Canva](https://www.canva.com/) uses our API to customise layouts.
    
-   **Graphics and text editors.**  [Gravit](https://gravit.io/)  allows to insert our icons via API into their mockups.
    
-   **Any application with customisation.**  [TimeTune](http://timetune.center/)  uses our API to customise activities.

