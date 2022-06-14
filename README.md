# searchbang

Search the web without search engines

My favourite search engine is https://duckduckgo.com. 
Other than its privacy it comes with an amazing feature of "Bangs" where you can redirect to search on the chosen website if we use specific word for it.

## Features

1. If you know the site bang you can put it without selection of menus to save time. If you don't you have menu to select it.
2. You can choose any browser to open the search link.
3. You can even disable auto opening of browser if you want and just get the URL.
4. In place of fzf you can chose rofi or dmenu if you like it more.
5. You can add your own sites if you want by changing bang.json file.
6. To save more time, it is not going to duckduckgo.com and the redirect to the chosen website, instead i made it go directly.

## Requirements

jq
sed
rofi or dmenu or fzf (please change the menu variable to 1, 2, and 3 accordingly)
awk
curl

## Installation

Download the above mentioned requirement first (if not present).
Download this repository or use git clone

```
git clone https://github.com/abhilash26/searchbang.git
cd searchbang 
chmod u+x searchbang
```

For repeated use it is better to add this script to the bin folder or any folder which exists in PATH variable.

## Usage

```
./searchbang
```
or

```
./searchbang <bang> <search terms>
```

## Swallowing 

If your DM (Desktop Manager) or WM (Window Manager) has swallow functionality use that.

or use https://github.com/salman-abedin/devour which I personally do. 
then for BROWSER variable use BROWSER="devour firefox" (if firefox for example)


## Customizations

You can decide to not open browser automatically if you desire by setting the OPENBROWSER variable to 0 
```
OPENBROWSER=0
```
Use your preferred browser binary with custom options as the BROWSER variable 
For example:  
```
BROWSER="brave --incognito"
```
I know people has massive love for their own menu system.
currently this script supports dmenu rofi and fzf

For rofi:
```
MENU=1
```
For dmenu:
```
MENU=2
```
For fzf
```
MENU=3
```
A lot of optimizations and UX is needed on this. 
Please help by creating pull requests.


