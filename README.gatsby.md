# Gatsby v2 Starter with local Wordpress via Docker

This starter is forked from
[gatsby-starter-wordpress](https://github.com/GatsbyCentral/gatsby-starter-wordpress)
and modified to use a local WordPress installation running in Docker.

> **WARNING**: Using `yarn upgrade` or `npm update` will break the site. See [GatsbyCentral/gatsby-starter-wordpress#36](https://github.com/GatsbyCentral/gatsby-starter-wordpress/issues/36) and [gatsbyjs/gatsby#10262](https://github.com/gatsbyjs/gatsby/issues/10262) for more info. Hopefully we'll have a resolution soon. - 19 Dec 2018

## Use it now

    gatsby new NAME https://github.com/GatsbyCentral/gatsby-starter-wordpress

* Edit `gatsby-config.js`, change `baseUrl`
  - Make sure you have at least 1 post and 1 page on your WordPress site
  - Make sure at least 1 post has at least 1 tag
* Rejoice
  - File any [issues here](https://github.com/GatsbyCentral/gatsby-starter-wordpress/issues)

### Known Limitations

* This is based on the [netlify starter](https://github.com/netlify-templates/gatsby-starter-netlify-cms) which uses [bulma](https://bulma.io). This adds 150KB to every built page.
* Your WordPress site must have at least 1 post with 1 tag, or the starter will crash
* Nested pages / categories will not render with nested pages
  - A WordPress page like `/about/team/` will render on Gatsby as `/team/`
  - Likewise for categories
  - Discussion here https://github.com/GatsbyCentral/gatsby-starter-wordpress/issues/24

## CSS Processing

This plugin uses [gatsby-plugin-purgecss](https://www.gatsbyjs.org/packages/gatsby-plugin-purgecss/) and [bulma](https://bulma.io/). The bulma build would otherwise be ~170K which adds 170K to each of your built HTML pages. However, with purgecss this is reduced 90%.

## Original Sources

This project was based on the following resources.

[GatsbyCentral](https://www.gatsbycentral.com/) 
[gatsby-starter-wordpress](https://github.com/GatsbyCentral/gatsby-starter-wordpress)
[gatsby-starter-netlify-cms](https://github.com/netlify-templates/gatsby-starter-netlify-cms)

* https://github.com/tomByrer
* https://github.com/dajocarter