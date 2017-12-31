# Garna - WordPress theme
There are only two files absolutely required in a WordPress theme:
* index.php – the main template file
* style.css – the main style file
Though not required, you may see additional files in a theme’s folder including:
* PHP files – including template files
* Localization files
* CSS files
* Graphics
* JavaScript
* Text files – usually license info, readme.txt instructions, and a changelog file


## Files Structure
assets (dir)
      - css (dir)
      - images (dir)
      - js (dir)
inc (dir)
template-parts (dir)
      - footer (dir)
      - header (dir)
      - navigation (dir)
      - page (dir)
      - post (dir)
404.php
archive.php
comments.php
footer.php
front-page.php
functions.php
header.php
index.php
page.php
README.txt
rtl.css
screenshot.png
search.php
searchform.php
sidebar.php
single.php
style.css

http://wphierarchy.com/  

## PHP Files and Structure
* index.php - The main template file. It is required in all themes.
* header.php for generating the site’s header
* footer.php for generating the footer
* sidebar.php for generating the sidebar
* comments.php - The comments template.
* front-page.php - The front page template is always used as the site front page if it exists, regardless of what settings on Admin > Settings > Reading.
* home.php - The home page template is the front page by default. If you do not set WordPress to use a static front page, this template is used to show latest posts.
* header.php - The header template file usually contains your site’s document type, meta information, links to stylesheets and scripts, and other data.
* singular.php - The singular template is used for posts when single.php is not found, or for pages when page.php are not found. If singular.php is not found, index.php is used.
* single.php - The single post template is used when a visitor requests a single post.
* single-{post-type}.php - The single post template used when a visitor requests a single post from a custom post type. For example, single-book.php would be used for displaying single posts from a custom post type named book. The index.php is used if a specific query template for the custom post type is not present.
* archive-{post-type}.php - The archive post type template is used when visitors request a custom post type archive. For example, archive-books.php would be used for displaying an archive of posts from the custom post type named books. The archive.php template file is used if the archive-{post-type}.php is not present.
* page.php - The page template is used when visitors request individual pages, which are a built-in template.
* page-{slug}.php - The page slug template is used when visitors request a specific page, for example one with the “about” slug (page-about.php).
* category.php - The category template is used when visitors request posts by category.
* tag.php - The tag template is used when visitors request posts by tag.
* taxonomy.php - The taxonomy term template is used when a visitor requests a term in a custom taxonomy.
* author.php - The author page template is used whenever a visitor loads an author page.
* date.php - The date/time template is used when posts are requested by date or time. For example, the pages generated with these slugs:
http://example.com/blog/2014/
http://example.com/blog/2014/05/
http://example.com/blog/2014/05/26/
* archive.php - The archive template is used when visitors request posts by category, author, or date. Note: this template will be overridden if more specific templates are present like category.php, author.php, and date.php.
* search.php - The search results template is used to display a visitor’s search results.
* attachment.php - The attachment template is used when viewing a single attachment like an image, pdf, or other media file.
* image.php - The image attachment template is a more specific version of attachment.php and is used when viewing a single image attachment. If not present, WordPress will use attachment.php instead.
* 404.php - The 404 template is used when WordPress cannot find a post, page, or other content that matches the visitor’s request.

## CSS Files and Structure
* style.css – The main stylesheet. It is required in all themes and contains the information header for your theme.
* rtl.css - The right-to-left stylesheet is included automatically if the website language’s text direction is right-to-left.

#### style.css
/*
Theme Name: Garna
Theme URI: https://wordpress.org/themes/garna/
Author: Artem Horbenko
Author URI: https://horbenko.com/
Description: Garna brings your site to life with immersive featured images and subtle animations. With a focus on business sites, it features multiple sections on the front page as well as widgets, navigation and social menus, a logo, and more. Personalize its asymmetrical grid with a custom color scheme and showcase your multimedia content with post formats. Our default theme for 2017 works great in many languages, for any abilities, and on any device.
Version: 1.0
License: GNU General Public License v2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html
Text Domain: garna
Tags: one-column, two-columns, right-sidebar, flexible-header, accessibility-ready, custom-colors, custom-header, custom-menu, custom-logo, editor-style, featured-images, footer-widgets, post-formats, rtl-language-support, sticky-post, theme-options, threaded-comments, translation-ready
This theme, like WordPress, is licensed under the GPL.
Use it to make something cool, have fun, and share what you've learned with others.
*/

## Child Theme

##  Features
* Site Header
  * Site title
  * Custom logo
  * Headere Menu Nav
  * Header Search
  * Headere Socials Nav
* Main content
  * Typography
    * Headings
    * Text
    * Blockquotes
    * Lists
    * Images
    * Tables
  * Components
    * Breadcrumb
    * Buttons
    * Carousel / Slider
    * List group
    * Pagination
  * Templates
    * Home
    * About
    * Contacts
    * Typography
    * Projects Archive
    * Page
    * Single
    * Archive
    * Search
    * 404
  * Layout
    * Full width
    * Full width 2 columns
    * Left sidebar
  * Shortcodes
    * Full width Slider
    * Carousel
    * iBoxBottom
    * iBoxRight
    * Latest Posts
    * Projects Loop
    * Team Loop
    * Partners Loop
  * Modules
    * Services
    * Process
    * Contactform
    * Google Map
    * Google Calendar
    * Comments
  * template-parts
    * content-none
    * content
    * content-page
    * content-search
    * content-decks
    * content-masonry
  * Customizer
* Site Footer
  * Footer Menu Nav
  * Footer Widgets Area
  * Terms of Use & Copyright
  
## Post types
* Post (Post Type: ‘post’)
* Page (Post Type: ‘page’)
* Attachment (Post Type: ‘attachment’)
* Revision (Post Type: ‘revision’)
* Navigation menu (Post Type: ‘nav_menu_item’)

### Custom post types
+ Projects
+ Team
+ Partners
+ Events


## Post Formats
The following Post Formats are available for users to choose from Garna theme.
* Standard - When writing or editing a Post, Standard is used to designate that no Post Format is specified. Also if a format is specified that is invalid then standard (no format) will be used.
* Aside - Typically styled without a title. Similar to a Facebook note update.
* Gallery - A gallery of images. Post will likely contain a gallery shortcode and will have image attachments.
* Link - A link to another site. Themes may wish to use the first <a href=””> tag in the post content as the external link for that post. An alternative approach could be if the post consists only of a URL, then that will be the URL and the title (post_title) will be the name attached to the anchor for it.
* Image - A single image. The first <img /> tag in the post could be considered the image. Alternatively, if the post consists only of a URL, that will be the image URL and the title of the post (post_title) will be the title attribute for the image.
* Quote - A quotation. Probably will contain a blockquote holding the quote content. Alternatively, the quote may be just the content, with the source/author being the title.
* Status - A short status update, similar to a Twitter status update.
* Video - A single video or video playlist. The first <video /> tag or object/embed in the post content could be considered the video. Alternatively, if the post consists only of a URL, that will be the video URL. May also contain the video as an attachment to the post, if video support is enabled on the blog (like via a plugin).
* Audio - An audio file or playlist. Could be used for Podcasting.
* Chat - A chat transcript, like so:

## Functions
* Theme Setup
* Automatic Feed Links
* Navigation Menus
* Load Text Domain
* Post Thumbnails
* Post Formats
* Initial Setup
* Content Width
...

## Custom template tags
* posted on
* posted by
* category snd tagged
* feature image
* posts navigation
* archive navigation
* breadcrumps

### Source:
* https://help.market.envato.com/hc/en-us/articles/202500774-ThemeForest-General-File-Preparation-Guidelines
* https://help.market.envato.com/hc/en-us/articles/202822450-WordPress-Theme-Submission-Requirements
* https://developer.wordpress.org/themes/getting-started/
* https://codex.wordpress.org/Theme_Development
* https://github.com/Automattic/_s