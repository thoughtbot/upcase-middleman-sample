Upcase Middleman Sample
=======================

This repo contains a sample project build with the [Middleman][] static site
generator. This project was built for [a video on Upcase][], our learning
platform.

[Middleman]: https://middlemanapp.com/
[a video on Upcase]: https://upcase.com/videos/building-static-sites-with-middleman

Getting Started
---------------

The repo includes a setup script that you can run to get started. Run the
script with:

``` sh
$ bin/setup
```

This will install the dependencies via `bundler` and copy over a template
`.env` file.


Running
-------

To run the app locally, run:

``` sh
$ middleman server
```

This will start the server with a file watcher and live reload functionality.


Deploying
---------

You'll need to set up an [S3 bucket][] to store the content and configure
[website hosting][] for the bucket, as well as populating the `.env` file
with your AWS keys and bucket name.

Once you have that in place, you can deploy (and re-deploy) with:

``` sh
$ bin/deploy
```


[S3 bucket]: https://aws.amazon.com/s3/
[website hosting]: http://docs.aws.amazon.com/AmazonS3/latest/dev/WebsiteHosting.html
