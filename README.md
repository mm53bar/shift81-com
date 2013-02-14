Shift81.com
===========

This is the source code for the [shift81.com](http://www.shift81.com) website.

It is designed to be built locally and deployed to Amazon S3 for use with Cloudfront.

Install
=======

Want to make your own site?  Easy peasy.

     git clone git://github.com/Shift81/shift81-com.git mysite-com
     cd mysite-com
     bundle install
     cp .env-sample .env

Now update `.env` with your information.  After that, build the site and enjoy!

     bundle exec foreman run middleman build

Amazon AWS
==========

You'll need to create a bucket on Amazon S3 and configure it as a website.  [Amazon has great instructions for this](http://docs.aws.amazon.com/AmazonS3/latest/dev/HostingWebsiteOnS3Setup.html).

At this point, you should be able to view your website using the website endpoint that S3 provides you.  But if you want to take it a bit further, set up Amazon Cloudfront.  Once again, [Amazon is the place to get the documentation](http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/CreatingDownloadDistributions.html).

Thanks
======

Thanks to the following authors and projects that are all rolled up together in this website:

* [holman/left](https://github.com/holman/left)
* [middleman/middleman](https://github.com/middleman/middleman)
* [middleman/middleman-blog](https://github.com/middleman/middleman-blog)
* [karlfreeman/middleman-sync](https://github.com/karlfreeman/middleman-sync)
* [fog/fog](https://github.com/fog/fog)
* [ddollar/foreman](https://github.com/ddollar/foreman)
