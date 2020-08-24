# Valtech WebAR Demo

With modern smartphones it is now possible to deliver performant AR experiences from the browser using web technologies.

If you combine this with QR codes you can deliver cross-browser AR experiences with very low user friction.

# Technology

This project utilizes [PlayCanvas](https://playcanvas.com/).

# Contributing

This project is hosted on Github Pages and is using Jekyll to build the site. It is recommended that you use rbenv for your Ruby and GEM environment. Here is a decent [guide](https://jekyllrb.com/docs/installation/) if you need help setting up Ruby.

To set up your development environment first run the following from the project root directory:

`$ bundle install`

To build the site and make it available on a local server:

`$ bundle exec jekyll serve`

In order to achieve camera access when running on localhost, you need an HTTPS certificate. You can build the certificate following the 'with Jekyll' instructions [here](https://dev.to/remotesynth/running-ssl-on-localhost-42ol).
Once you have generated the localhost.key and localhost.crt files in the project directory, you can then run (make sure to use https, https://localhost:4000):

`$ bundle exec jekyll serve --ssl-key localhost.key --ssl-cert localhost.crt`


# Usage

You need to print out or display a tracking marker on another device. It can be found [here](https://webar.valtech.engineering/assets/images/qr-code.png).

Once you enter the AR experience (preferably with a mobile device) you should be prompted for camera access (unless you're on iOS and not in Safari, in which case this won't work). Upon approval, the camera stream is looking for the tracking marker. Move the camera close to the marker until the 3D coat appears above it.