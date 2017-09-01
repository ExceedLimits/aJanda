# aJanda - v0.1

Simple Event Agenda (RTL is Supported) - by [joory](http://www.joory.me/).

### Synopsis

it is a cool element, not many of it's kind are found out there, all conference websites need a decent schedule displayed in style.

### Motivation

i needed it, so i made it, Feel free to use it too.

## Getting Started

Simple steps are needed, it is too easy to install and use:

### Prerequisities

Only [JQuery](https://code.jquery.com/), Goes without saying.

### Installing

Fisrt, You need to download all files as zip File. 

then, add those haeder references **(after JQuery)**:

```html
<link href='./your_css_folder/aJanda.css' rel='stylesheet' type='text/css'/>
<script src='./your_js_folder/aJanda.js'></script>
```

that is it, installation is done. 

## Usage

start by picking the right element to host a new aJanda instance, multiple options are available:

```javascript
$(document).ready(function() {
                $('.hostelement').aJanda({		 
                    darkColor: '#545f60',
                    mainColor: '#3498db',
                    schedule:[
                        {date:"2017/05/13 01:00 PM",title:"ttl1",content:"sample content1"},
                        {date:"2017/05/13 09:00 AM",title:"ttl2",content:"sample content2"},
                        {date:"2017/05/12 10:00 AM",title:"ttl3",content:"sample content3"},
                        {date:"2017/05/12 11:00 AM",title:"ttl4",content:"sample content4"},
                        {date:"2017/05/12 01:00 PM",title:"ttl5",content:"sample content5"}
                    ],
                }); 
            });
```
## Options Reference

the Option List helps you customize Style and Content:

###Theme
use `darkColor` , `lightColor` , `mainColor` , `bgColor` to Customize aJanda theme. set using HEX color format.

###Html Content
set `htmlContent` to Enable adding your own html code as content. **False by default** 

###RTL Support
set `RTL` to Enable RTL layout. **False by default** 

###Locale Support
set `Locale` to choose your desired Localization. **'en-us' by default** 

###Schedule
use `date` , `title` , `content` to add aJanda segments.
for more customizations set `extraClass` with your CSS Classes (**use !important if needed**)
**make sure you have a non-empty schedule** 

###Titles
you can assign Tiltes for each Day, just Fill the right ammount of `Titles` array.

Here is a Full Example:
```javascript
$('.hostelement').aJanda({		 
                    darkColor: '#545f60',
                    mainColor: '#3498db',
                    lightColor: '#6edeef',
                    bgColor: '#ffffff',
                    htmlContent: false,
                    RTL:false,
                    Locale:'en-us',
                    schedule:[
                        {date:"2017/05/13 01:00 PM",title:"ttl1",content:"sample content1",extraClass:"myclass"},
                        {date:"2017/05/13 09:00 AM",title:"ttl2",content:"sample content2"},
                        {date:"2017/05/12 10:00 AM",title:"ttl3",content:"sample content3"},
                        {date:"2017/05/12 11:00 AM",title:"ttl4",content:"sample content4"},
                        {date:"2017/05/12 01:00 PM",title:"ttl5",content:"sample content5"}
                    ],
                    Titles:["First Day","Second Day"]
                });
```

## Built With

* JQuery
* Brackets IDE

## License

This project is licensed under The MIT License (MIT) - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

* [joory](http://www.joory.me/)
