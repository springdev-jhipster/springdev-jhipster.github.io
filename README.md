这里是 JHipster 中文网站，由 [Spring 技术社区](https://springdev.io)维护。
JHipster 的官方网站，请点击 [这里](https://www.jhipster.tech/).
=======

This Web site is rendered with GitHub pages.

To run this locally

* [Fork this](https://github.com/jhipster/jhipster.github.io/fork) repo and clone to your file system
* [Install Jekyll](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/)
* Run `bundle install` if you are running it for the first time.
 * If you want to avoid installing to system directories, install to vendor directory instead: `bundle install --path vendor/bundle`
 * On MacOS, if you have trouble installing `nokogiri`, try: `bundle config build.nokogiri --use-system-libraries=true --with-xml2-include="$(xcrun --show-sdk-path)"/usr/include/libxml2`
* Run `bundle exec jekyll serve` in the cloned repo folder
* You will be able to access the site at http://localhost:4000

Or with Docker and Docker-Compose (recommended way on Windows)

* [Fork this](https://github.com/jhipster/jhipster.github.io/fork) repo and clone to your file system
* Run `docker-compose up`
* You will be able to access the site at http://0.0.0.0:4000
