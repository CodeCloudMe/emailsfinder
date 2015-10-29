This is an email address scraper, which seeks to take a topic input and return relevant e-mail addresses geared towards that topic.
This script will Bing search the input at http://localhost:8080/?subject=bitcoin, search for bitcoin, and based on the limit you set, it will search through that many pages of results and extract e-mails from the sub pages of all the pages found in the search.

Looking forward to improving this to make e-mail responses much more relevant and getting it to run a little better on OpenShift.

To run:

git clone http://github.com/codecloudme/emailsfinder

cd emailsfinder

npm install

node server.js

This runs on port 8080.

The main code is in server.js and lib/mailing/index.html


This is built to run in an openshift environment. Feel free to import this repo directly to Openshift; however, there are some bugs, which we hope to resolve. 

The OpenShift `nodejs` cartridge documentation can be found at:

http://openshift.github.io/documentation/oo_cartridge_guide.html#nodejs


[![Join the chat at https://gitter.im/CodeCloudMe/emailsfinder](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/CodeCloudMe/emailsfinder?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)