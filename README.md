# Valtech WebAR Demo

With modern smartphones it is now possible to deliver performant AR experiences from the browser using web technologies.

If you combine this with QR codes you can deliver cross-browser AR experiences with very low user friction.

# Technology

This project utilizes [AFrame](https://aframe.io) and [AR.js](https://github.com/AR-js-org/AR.js).

# Contributing

This project is hosted on Github Pages and is using Jekyll to build the site. It is recommended that you use rbenv for your Ruby and GEM environment. Here is a decent [guide](https://jekyllrb.com/docs/installation/) if you need help setting up Ruby.

To set up your development environment first run the following from the project root directory:

`$ bundle install`

To build the site and make it available on a local server:

`$ bundle exec jekyll serve`

In order to achieve camera access when running on localhost, you need an HTTPS certificate. You can build the certificate following the 'with Jekyll' instructions [here](https://dev.to/remotesynth/running-ssl-on-localhost-42ol).
Once you have generated the localhost.key and localhost.crt files in the project directory, you can then run:

`$ bundle exec jekyll serve --ssl-key localhost.key --ssl-cert localhost.crt`