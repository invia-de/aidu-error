# AIDU Emergency Frontpage

Emergency website shown via S3 if AIDU is completely offline.

## About

This website is being deployed using Gitlab CI to [AWS S3](http://ab-in-den-urlaub-fallback.s3-website.eu-central-1.amazonaws.com/) ([Cloudfront](https://d1e2n8ff33k5hc.cloudfront.net/)) for each tag. (Not working as of yet, as it needs data credentials for AWS).
All other commits are published to [Gitlab Pages](https://shared-travel-packages.gitlab-pages.invia.io/aidu-whitelabel/emergency/).

## Usage

Once an emergency happens Cloudflare *should* display the page automatically for [ab-in-den-urlaub.de](ab-in-den-urlaub.de).

All other whitelabels must be redirected via DNS by IT Operations, these whitelabels are as of now (2019/10/10):

* ab-in-den-urlaub.ch
* ab-in-den-urlaub.at
* reisegeier.de
* reisegeier.ch
* reisegeier.at
* reisen.de
* reisen.fluege.de
* travelchannel.de

It's recommended to switch the DNS for ab-in-den-urlaub.de too, as Cloudflare seems not to provide their "Always On" feature as advertised.