# website imkereigrunert.de

## install

* create a new hugo site `hugo new site <sitename>`
* switch into the new directory: `cd <sitename>`
* clone the `hugo-scroll` theme repository: `git clone https://github.com/magomi/hugo-scroll.git themes/hugo-scroll`
* switch into the `hugo-scroll` directory: `cd themes/hugo-scroll`
* init/update the submodule: `git submodule init`, `git submodule update`

## run locally

* cd into the theme directory: `cd <site>/themes/hugo-scroll` 
* serve the site locally: `hugo server --source=website_imkerei --themesDir=../..` 
* access the site on `http://localhost:1313`

## build and publish

* build the site: `hugo --source=website_imkerei --themesDir=../..`
* sync to the server: `rsync -av ./website_imkerei/public/* <user>@www.imkereigrunert.de:/var/www/imkereigrunert.de`

## notes

Not clear how to better separate between hugo site, theme (hugo-scroll) and content. Content should be served from the site directory. Either I need to figure out how to do this or if another template fits better with my usecase.
