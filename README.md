# website imkereigrunert.de

# install

* create a new hugo site `hugo new site <sitename>`
* switch into the new directory
* remove the git tracking, will not be used (can be regenerated any time)
* clone the `hugo-scroll` theme repository: `git clone https://github.com/magomi/hugo-scroll.git themes/hugo-scroll`
* switch into the `hugo-scroll` directory
* init/update the submodule: `git submodule init`, `git submodule update`
* build the site: `hugo --source=website_imkerei --themesDir=../..`
* sync to the server: `rsync -av ./website_imkerei/public/* <user>@www.imkereigrunert.de:/var/www/imkereigrunert.de`



