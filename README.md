# aJanda - v1.0

Simple Event Agenda (RTL is Supported)

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
## API Reference



## Built With

* JQuery
* Brackets IDE

## License

This project is licensed under The MIT License (MIT) - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

* [joory](http://www.joory.me/)
