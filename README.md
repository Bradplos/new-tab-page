#new-tab-page

new-tab-page is a simple, customisable offline browser site which allows you to create a quickly accessible list of websites. new-tab-page uses a text-format model, meaning that all links are visible to you, allowing for quicker navigation to your a desired website.

<br>
## Configuration

#### HTML
Categories are created like this within the container _div_, where __TITLE__ is your category name

```
<span class="title">TITLE</span>
  <span class="seperator-1">&nbsp; >> &nbsp;</span>
```
Links are created like this after your category, where __EXAMPLE__ is your link name, and the __id__ matches the one with the link in _main.js_
```
<a id="google"><span class="link">EXAMPLE</span></a>
  <span class="seperator-2">-</span>

<a id="yahoo"><span class="link">EXAMPLE</span></a>
  <span class="seperator-2">-</span>

<a id="bing"><span class="link">EXAMPLE</span></a>
  <span class="seperator-2">-</span>
```

#### JS
To create or change new links, follow this format:
`$('#').attr('href','URL');`
where whatever follows the __#__ is your id, and the __URL__ is your desired URL.

```
$('#google').attr('href','https://google.com');
$('#yahoo').attr('href','https://yahoo.com');
$('#bing').attr('href','https://bing.com');
```

#### Change the Search service
Find
```
<form method="get" action="https://www.startpage.com/do/search?q=" class="search-bar">
```
And change the insides of `action=" "` to your desired search service. Startpage is active by default.

- Google: `https://www.google.com/#q=`
- Startpage: `https://www.startpage.com/do/search?q=`
- DuckDuckGo: `https://duckduckgo.com/`

<br>
## Installation

### Download
To download new-tab-page, either
- [Download the zip](https://github.com/Bradplos/new-tab-page/archive/master.zip)
- Clone the repo: `git clone https://github.com/bradplos/new-tab-page.git`


### What is in the download?
Keep the following all in the same folder and positions
```
new-tab-page/
├── index.html
├── style.css
├── main.js
```

### Install

####Firefox
##### To set as a homepage
- Open a new tab __->__ go to 'about:preferences' __->__ General __->__ Startup __->__ Home Page: __->__ Set as your_folder_location/new-tab-page/index.html


#####To set as a new tab
- Open a new tab __->__ go to 'about:config' __->__ search for 'browser.newtab.url' __->__ set as your_folder_location/new-tab-page/index.html


<br>
## License
All of new-tab-page is free to use and abuse under the [open-source MIT license](https://raw.githubusercontent.com/Bradplos/new-tab-page/master/LICENSE).
