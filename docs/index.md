# Welcome to icons user manual
This document covers pretty much everything you need to know about how to get started and succeed with icons services.

# Why the Icons8?

The demand for visual content seems is only getting stronger nowadays. Having just a huge bunch of icons files may not necessarily help one to efficiently and competitively develop and support visually rich applications. Wouldn't it be much more better to have a dedicated reliable platform like the [Icons8](https://icons8.com/) that would cope with all sort of the challenges associated with managing icons, keeping them up-to-date, and making them easily accessible in the most suitable forms and various contexts?

# Which license do I need?

Conceptually, the [Icons8](https://icons8.com/) provides two frameworks or in other words two distinct ways of how icons could be accessed and utilized. These two licensing pathways are known as <b>['Standard'](#standard-framework) and ['Service Integration'](#service-integration-framework) frameworks</b>. Each framework is associated with certain set of tools which are discussed below in detail. 

<!--
One of the most frequently asked questions from our customers is "<b>which license do I need</b>", meaning <b>which framework am I supposed to use</b> to achieve the goals of my project. The rest of this document is purposely dedicated to give you a clear answer for that question and to master the essentials of the frameworks. -->

  

## Service Integration Framework
In a short, service integration gives you an ability to access icons programmatically, from within your apps, on the fly in real-time. In particular end-users of your products could generate their own projects, build their own visual content from within your apps tied to our service. The framework consist of:

<!--<ul>
  <li>-->
   <details>
  
  <summary>
   <strong>Search Engine</strong>
  </summary>
  
  
 <!--## Overview-->
 
 <ul>
  <li>
   <details>
    <summary>
      <strong> How to to search for icons metadata? </strong>
    </summary>
 Requests to the <b>Search Engine</b> are constracted with the use of your API KEY, set of paramters, concatenated one after another (order could be changed on you own) in a raw and prefixed with the endpoint for the service. Here is a sample request: https://api.icons8.com/api/iconsets/v4/search?term=home&amount=50&offset=0&platform=all&language=en-US&token=al05i21yfatb4s5eac20c4wr4394b1z2. 
     
   </details> 
  </li>
  <li>
   <details>
    <summary>
      <strong> Searching Parameters </strong>
    </summary>
     
     ### Platform Parameter

Attributes and parameters named  `platform`  or  `platform_api_code`  or  `platform_code`  all indicate the style of the icons. We are sorry, we have various names which mean the same things.

|Platform|Icon style|
|----------|--------|
|win8|icons in the Microsoft Windows 8/Metro style| 
|win10 |icons in the Microsoft Windows 10/Threshold|
|ios7|icons in the Apple iOS 7/8/9/10 style|  
|android|icons in the Google Android 4 Kitkat style| 
|androidL|icons in the Google Android 5 Lollipop (Material) style| 
|color|flat color icons| 
|office|icons in the Microsoft Office style| 
|ultraviolet|Ultraviolet|				
|nolan|Nolan|				
|p1em|1em|
|dotty|	Dotty Dots|	
|dusk|Dusk|				
<!--
75	Dusk_Wired	Wired	✓			✓	Update
140	cotton	Cotton				✓	Update
12	ios11	iOS Tab Bar Icons (Glyphs)	✓			✓	Update
301	clouds	Clouds				✓	Update
302	bubbles	Bubbles				✓	Update
303	plasticine	Plasticine				✓	Update
304	carbon_copy	Carbon Copy	✓			✓	Update
250	doodle	Doodle				✓	Update
251	fineline	Fune Line					Update
252	isometric	Isometric					Update
253	flat_round	Flat Round				✓	Update
14	m_outlined	Material Outlined	✓		/static/effects/svg/icons/androidL/	✓	Update
15	m_rounded	Material Rounded	✓		/static/effects/svg/icons/androidL/	✓	Update
16	m_two_tone	Material Two Tone				✓	Update
17	m_sharp	Material Sharp	✓		/static/effects/svg/icons/androidL/	✓	Update
|linen|Linen|

-->

### Language Parameter

Icon names, categories and tags are localized. Here's the list of supported languages:

|Language|Language name|
|----------|--------|
|en-US|English|
|fr-FR|French|
|de-DE|German|
|it-IT|Italian|
|pt-BR|Portuguese|
|pl-PL|Polish|
|ru-RU|Russian|
|es-ES|Spanish|
|zh-CN|Chinese|
|ja-JP|Japanese|

The primary language is English - if we do not translate something, it will be in English.

### Amount Parameter
The maximum number of icons which you'd like to receive. Default value is 25

### Offset Parameter
The offset from the first received result. Default value is 0

    </details>
   </li>
   <li>
    <details>
     <summary>
       <strong> sample JSON returned by the service </strong>
     </summary>
      
 |<img src='https://github.com/visualpharm/icons-docs/blob/master/docs/Images/v4_Search_JSON_1.png'>|<img src='https://github.com/visualpharm/icons-docs/blob/master/docs/Images/v4_Search_JSON_2.png'>|
|----------|--------|
     </details>
    </li>
 
Notice that you can filter results with style/platform and then group the results with the use of categories. Basically when you supply a search query to our <b>Search Engine of Version 4.0</b> you get back a json file which contains all the metadata of the most relevant icons associated with that query. Then you may use this category info contained in the metadata to actually group the results according to the categories.

Please pay attention that the <b>Search Engine</b> will not return the categories which have less than 10 icons.





 </details>
    
 
  
  <br>
  
  <details>
  <summary>
   <strong>Retrieval Engine</strong>
    
  </summary>

<br> 
  <b>Icons Retrieval Service</b> could be used as a stand along absolutely <b>FREE</b> service. Paid access gives you <b>unbeatable</b> functionality to craft cutting edge apps.  

<ul>
  <li>
   <details>
    <summary>
      <strong> How to retrieve an icon? </strong>
    </summary>
 Everything becomes much more easier with [omg-img](http://img.icons8.com/) service. For example, it takes just a line of code `<img src=’https://img.icons8.com/search’/>` to insert a png icon [Magnifier](https://icons8.com/icon/set/magnifier/all) directly from the CDN to your application of any scale.
     
   </details> 
  </li>
  <li>
   <details>
    <summary>
      <strong> Free VS Paid </strong>
    </summary>
    
Most of the [omg-img](http://img.icons8.com/) features are available to our clients for free. Of cause there are advanced options available only to licensed clients. The major difference is that API license provide extra features which are:
- functionality to generate PNG icons larger than 550 px
- access to vector-format icons (SVG, EPS, PDF)
The possibility to request a large number of items in any size, color or format
The possibility to search for icons using our search engine 2.
   </details> 
  </li>
  <li>
   <details>
     <summary>
       <strong> Icon’s search available straight from the address bar of your browser</strong> 
     </summary>
   
For your convenience, [omg-img](http://img.icons8.com/) service architecture allows developers and designers to browse for new icons directly from browser’s address bar as following: 
 - https://img.icons8.com/home 
 - https://img.icons8.com/house
- https://img.icons8.com/bungalow
- https://img.icons8.com/targaryen-house
There is always an option to browse for more icons from our web site search engine UI  https://icons8.com/icon/new-icons/all to get the names that you may use in constructing appropriate icons links for your apps.
   </details>  
   
  </li>
  <li>
   <details>
    <summary>
      <strong>How do I apply styles?</strong>
    </summary>
  
On our website, there is a list of icons styles on the left pane of the icons page. The list contains more than 20 various styles to outperform expectations of even the most demanding end-users of your apps. Below is the list of the most popular styles:

|monochrome|coloured|
|----------|--------|
|iOS: http://img.icons8.com/ios/car|Color: http://img.icons8.com/color/car|
|Windows: http://img.icons8.com/windows/car|Office: http://img.icons8.com/office/car|
|Material: http://img.icons8.com/material/car|Dusk: http://img.icons8.com/dusk/car|

[Omg-img](http://img.icons8.com/) let you apply a new style as easy as just inserting a style code within an icon’s link.
 </details>
 
   </li>
 </ul> 
  

**4. Recolouring monochrome icons made easy**
To change the color of an icon with [omg-img](http://img.icons8.com/) service you simply insert an appropriate color code within an icon’s link as it is demonstrated below:
- <img src='http://img.icons8.com/ios/FF0000/car'> `http://img.icons8.com/ios/FF0000/car`
- <img src='http://img.icons8.com/ios/00FF00/car'> `http://img.icons8.com/ios/00FF00/car`
- <img src='http://img.icons8.com/ios/0000FF/car'> `http://img.icons8.com/ios/0000FF/car`

**5. How can I resize an icon?**
To modify an icon’s size the same logic is applied as before. It’s just enough to insert an icon’s size within its link:
- 'http://img.icons8.com/color/30px/car' <img src='http://img.icons8.com/color/30px/car' />
- 'http://img.icons8.com/color/40px/car' <img src='http://img.icons8.com/color/40px/car' />
- 'http://img.icons8.com/color/50px/car' <img src='http://img.icons8.com/color/50px/car' /> 
- 'http://img.icons8.com/color/60px/car' <img src='http://img.icons8.com/color/60px/car' /> 

For your convenience, the size of an icon can be written in two different formats: `100x100` or `100px`, depending on what you prefer the most.

**6. How can all sorts of artefacts be minimised when using pixel perfect?**
Each icon style is drawn for a specific pixel grid. Look at these few examples of various pixel grids: 
* iOS: `50x50`
* Metro: `26x26`
* Windows: `32x32`
* Material: `24x24`
* Color: `48x48`
* Office: `16x16`, `30x30`, `40x40`, `80x80`

In order to avoid all sorts of artefacts (blurring edges, washed out colours etc.) associated with changing an icon’s size, we strongly recommend you to choose multiples of original icon's size. For example for iOS style the multiples would be: `50x50`, `100x100`, `150x150` etc.
You can set an icon’s size either by specifying the size in pixels `100x100` / `100px` or with the use of factors: `2x` or `x2` (the number can vary).
For example:
- 'https://img.icons8.com/color/1x/brazilian-carnival.png' <img src='https://img.icons8.com/color/1x/brazilian-carnival.png'/>
- 'https://img.icons8.com/color/2x/brazilian-carnival.png' <img src='https://img.icons8.com/color/2x/brazilian-carnival.png' />

**7. What is the maximum size of an icon that your service can provide?**
The restriction applied to free png icons is 550px. Please read more in [API license](https://icons8.com/paid-license-99/#/).

**8. Which license do I need to start using [omg-img](http://img.icons8.com/)?**
To start using [omg-img](http://img.icons8.com) service for free, just [set a link](https://icons8.com/license) or buy [paid licence](https://icons8.com/paid-license-99/#/).

**9. What should I do if I can not find an icon that I need?**
You may send us a [request](https://icons8.com/request-icon/) to draw any icon you actually  need. It’s completely free. We try to do our the best to make our service comprehensive. However we do prioritise the requests which have the highest demand. You even may ask your friends, relatives and any community members to vote for your requested icon in order put your request on the very top of the queue. 

**10. Can an icon used in my app change over time?**
In short, it’s very unlikely but possible. The most updated version of an icon is accessible by a given icon’s link.
E.G. currently for the following link **`https://img.icons8.com/water-molecule`** we keep showing an icon with illustration of a water drop or an abstract molecule. However if we begin to receive more and more requests to change the icon’s appearance to say a water molecule like this H<sub>2</sub>O, then most probably we will alternate its look somehow to represent the structure of two atoms of hydrogen and one atom of oxygen bonded together. 

In case if you are planning to use an icon longterm, the best solution would be to use the canonical full path to the icon (.png), which can be formed [here](https://icons8.com/).

**11. Can I use an icon with .png extension?**
Yes you can use icons with .png extension in [omg-img](http://img.icons8.com/) service, however you would need to know the exact name of a .png icon. The .png names could differ from the names provided by the service. In order to find the desired .png icon name and create an appropriate query for it, you may use searching engine UI available on our website [here](https://icons8.com/icon/new-icons/all).

**12. How to use responsive size for [Office](https://icons8.com/office-icons/) style?**
It’s quite simple. Just add a parameter `office` to your request. For example:
 - <img src='http://img.icons8.com/office/50px/car.png?office=16'> `http://img.icons8.com/office/50px/car.png?office=16`
- <img src='http://img.icons8.com/office/50px/car.png?office=30'> `http://img.icons8.com/office/50px/car.png?office=30`
- <img src='http://img.icons8.com/office/50px/car.png?office=40'> `http://img.icons8.com/office/50px/car.png?office=40`
- <img src='http://img.icons8.com/office/50px/car.png?office=80'> `http://img.icons8.com/office/50px/car.png?office=80`


<br>
 </details>
 
 
<!-- </li>
 </ul>
</details> 
<br>-->

<br>

<b>Search Engine</b> allows to programmatically search for icons metadata, whereas <b>Icons Retrieval Service</b> utilizes that metadata to actually retrieve icons in various formats, styles, colours, sizes etc. <b>Click on the collapsible items above to read more details about each of the services.</b> The <b>Licensing Model</b> for the <b>Service Integration Framework</b> can be viewed by clicking on the item below:
 
  <details>
  <summary>
   <strong>Licensing</strong>
  </summary>
  
  <br>
  ### License Expiration

- 
## Pricing / Getting Started

The starter icons Service Integration is $100/month - it includes up to 100 000 requests (actual, non cached icons downloads) per month. Every 100 000 requests add $100 more. After we receive a payment from you we'll issue an API key. You may proceed with the payment on this page: https://icons8.recurly.com/subscribe/api_access
  
 </details>
 <br>
 <details>
  <summary>
   <strong>Use Cases</strong>
  </summary>
  
  <br>

  These are examples of API usage in production applications:

-   **Template customisation.**  <br> This is how  [Canva](https://www.canva.com/) uses our API to customise layouts.
    
-   **Graphics and text editors.** <br>  [Gravit](https://gravit.io/)  allows to insert our icons via API into their mockups.
    
-   **Application customisation.** <br>  [TimeTune](http://timetune.center/)  uses our API to customise activities.

 </details>
 



## Standard Framework

Under the <b>Standard Framework</b> we consider a set of tools that allow our clients to manually search and retreive icons through some GUI. These tools are:
 
  <details>
  <summary>
   <strong>Web App</strong>
  </summary>
   
 ### Searching
 ...
### Editing/Formating
...
### Effects/Collections
...
### Downloading 
...

 </details>
   
<br>

  <details>
  <summary>
   <strong>Desktop Apps (Windows & Mac)</strong>
  </summary>
  
  <br>
 Desktop Apps (Windows & Mac)
 </details>
 
 <br>

Both <b>Web and Desktop Apps</b> have a very similar functionality with some distinctions that are <b>described in detailed in each of the collapsable items above</b>. The <b>Licensing Model</b> for the <b>Standard Framework</b> can be viewed by clicking on the item below:
 
  <details>
  <summary>
   <strong>Standard Framework Licensing Model</strong>
  </summary>
  
  <br>
  more details goes here ...
  
 </details>
 
 
  

<!--
 <details>
  <summary>
   <span style="color:blue"><strong>LICENSING MODEL</strong></span>
  </summary>
 This section aims to explain in detail various aspects of licensing and pricing for icons/photos services. While the strict [license agreement](https://icons8.com/download/Icons8_License.pdf) mainly focuses on the legitimacy of various types of usage, this chapter helps our clients to quickly grasp the main pricing features and wisely select the best possible usage option.

There are two possibilities for our clients to use [Icons8](https://icons8.com/) services: on a free basis and on a payable basis. Please note that we do provide lots fruitful things to use for free. Actually, among all the icons/photos services there are only two services that potentially could be payable: [regular icon license](https://icons8.com/paid-license-99/#/) and [API integrations license](https://icons8.com/paid-license-99/#/). All other services provided absolutely for free without any hidden costs. Of cause, there could be some requests from our clients for custom art/photo processing work, but in general [these](https://icons8.com/paid-license-99/#/) are the only two services that in principle could be payable.  For information regarding the free of charge usage please read the ['Free of charge licensing'](#free-of-charge-licensing) section below. Payable option of cause have the most ambitious capabilities. All the shades of licensing associated with paid licenses are described in ['Paid licensing'](#paid-licensing) section. 
## Free of charge licensing
All of the [Icons8](https://icons8.com/) icons/photos services and icons apps can be used for free except the API integration service. You are welcome to use them for free for personal or commercial use however it will require from you to reference us somewhere in an appropriate (publicly accessible) place of your product. In most cases it is enough to place a web link pointed to our website's main page or best of all, pointed directly to the icon you decided to use. Please note that the free icons can only be downloaded in PNG up to 100x100px. The [Popular Icons](https://icons8.com/icon/pack/free-icons/all) and [Logos](https://icons8.com/icon/pack/Logos/all) are free in all formats, including SVG.  

Below is the list of suggested places where you may set up a link:

 - Websites - we require linking from all pages where the icons are used. Please put the link in the footer if the icons are used on each page. A nice example:  
  
![](https://storage.crisp.chat/users/helpdesk/website/0387cc22-33e9-44e8-826f-c5c18d31fc81/15635e20-8c02-41d0-9b98-da3da95cf81b.png)  
  
 - Desktop software - please put the link in the About dialog
 - Mobile apps - please put the link in the About dialog and acknowledgment on
   the AppStore/Google Play page. If the application doesn’t have an
   About section, please reference [Icons8](https://icons8.com/) on the app page
 - Chrome App - please add the link to the description in the Chrome Web Store and (if it doesn't break your layout) somewhere in Settings   
 - WordPress plugin - please link on the Settings page of the plugin and the
   plugin page   
 - PDF, Excel, Word, any other document and also eBooks
   and printed editions - you can put the link anywhere in the document 
 - PC game - please put the link in the Credits section. And we would
   love to have a copy of the game, thank you :-)   
 - YouTube - please put the link in the description box   
 - eBay page - you can put the link in the footer   
 - Social network - please place the link in some of your posts
 - T-shirts, mugs, umbrellas etc. - put the link in some noticeable location of the product

##  Paid licensing

 </details>
 
 <hr>
 -->
 
# FAQ
 
 <details>
  <summary>
   <strong>Service Integration Framework. Licensing. Requests limits. API Key. Limitations. Use cases. What if ... </strong>
 </summary>
 
 <br>
 <ol>
  <li>
   <details>
    <summary>
      <strong>How can I purchase Service Integration API Key? What is included?</strong>
    </summary>
    
   The starter icons Service Integration is $100/month - it includes up to 100 000 requests (actual, non cached icons downloads) per month. Every 100 000 requests add $100 more. After we receive a payment from you we'll issue an API key. You may proceed with the payment on this page: https://icons8.recurly.com/subscribe/api_access
   </details>
 <hr>
 </li>
 <li>
 <details>
  <summary>
   <strong>What are the end points for icons Searching/Retrieval? Give me few examples, please!</strong>
 </summary>
  
 The endpoint for searching requests is: https://search.icons8.com/api/iconsets/v4/search for retrieval: http://img.icons8.com In order to serch / retrieve an icon you embed your API key just right into the requests: https://search.icons8.com/api/iconsets/v4/search?term=home&amount=50&offset=0&platform=all&language=en-US&token= "YOUR API KEY" http://img.icons8.com/ios/F0AC34/search.svg?token= "YOUR API KEY" You may change the order of parameters in you request accodring to the documantation. Notice that you can filter results with style/platform and then group the results with the use of categories. Basically when you supply a search query to our v4 service you get back a json which contains all the metadata of the most relevant icons associated with that query. Then you may use this category info contained in the metadata to actually group the results according to categories.
 </details>
  <hr>
</li>
 <li>
 <details>
  <summary>
   <strong>Why icon size is not icluded in metadata returned by Search Engine? Why Pixel Perfect?</strong>
 </summary>
  
Notice, the icons that we have are of a vector format and that is why they could be of any size. By this reason we do not include the icon's size in metadata. I.e. you can substitute any size in the request of a retrieval serivce and receive the corresponding png icon in the requested size. For icons retrieval we use [Omg-Img](...) service. To retrieve an icon you embed your API key just right into your request http://img.icons8.com/ios/F0AC34/search.svg?token= "YOUR API KEY" You may change the order of parameters in your request. Also keep in mind that due to the conversion of svg into png the "pixel perfect" come into play. To eliminate the artefacts of format conversion (from vector to raster) there is an appropriate size for each platform which you can then multiply by various factors 1x, 2x, 3x etc. to get the png size you need. 
 </details>
  <hr>
</li>
</ol> 

 </details>

<br>

<details>
  <summary>
   <strong>Standard Framework. Licensing. Free usage. Editing. Web / Desktop. Usage after cancelation. Distribution. </strong>
 </summary>
 
 <br>
 <ol>
  <li>
   <details>
    <summary>
      <strong>Can I use Icons8 for free?</strong>
    </summary>
    
   Yes, you can use our icons for free for personal or commercial use if you put a link to our website.
   Please note that the free icons can only be downloaded in PNG up to 100x100px. The Popular Icons and Logos are free in all 
   formats, including SVG. Alternatively, you can purchase a license to get all formats and use them without crediting us.
   </details>
 <hr>
 </li>
 <li>
 <details>
  <summary>
   <strong>Can I use the icons after my subscription is expired?</strong>
 </summary>
  
Yes, the icons that you've used while your subscription was active can be used indefinitely.
Kindly note that after you make subscription and it expires you are not able to use previously downloaded icons on our web or app (unless you've downloaded them to your device).
 </details>
  <hr>
</li>
 <li>
 <details>
  <summary>
   <strong>How can I purchase just a single icon?</strong>
 </summary>
  
Unfortunately we do not have such an option at the moment. The best solution would be to purchase a subscription for a month, then download as many icons as you need and eventually cancel the subscription. You truly may cancel your subscription at any time, no hidden costs, no tricks no stuff like that. After your subscription is canceled you may continue to use your icons in current or future commercial projects. These icons stay yours for good. Though there are few restrictions are applied: https://icons8.com/download/Icons8_License.pdf
 </details>
  <hr>
</li>




</ol> 








</details>
