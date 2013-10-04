# Clean My Archives

An easy-to-use shortcode for displaying post archives on your site.

The Clean My Archives plugin was developed because so many archives plugins were overly complicated.  I wanted something extremely simple to use that simply got the job done on my own [site's archives](http://justintadlock.com/archives).

Therefore, I created a simple `[clean-my-archives]` shortcode that you can place on any page (or any shortcode-ready area) and list your post archives by month and year.

This plugin also integrates with WordPress caching plugins.  So, long lists of archives can be cached for later use and loaded quickly.  If you have many years of blog posts, I highly recommend some sort of persistent caching or paginating your archives (see FAQ).

## Usage

Add the `[clean-my-archives]` shortcode to a shortcode-ready area, such as the page editor. That's it.  You have nothing more to do.

Some other examples:

	// Limit number of posts

	[clean-my-archives limit="100"]

	// Limit by year

	[clean-my-archives year="2013"]

	// Limit by month

	[clean-my-archives month="12"]

	// Load different post types

	[clean-my-archives post_type="post"]

	[clean-my-archives post_type="post, page"]

	// Pagination (via the post/page editor)

	[clean-my-archives year="2013"]
	<!-- nextpage -->
	[clean-my-archives year="2012"]
	<!-- nextpage -->
	[clean-my-archives year="2011"]

## Changelog

### Version 0.2.0

* Use `wp_reset_postdata()`, not `wp_reset_query()`.
* Smarter code formatting for day and comments number.
* Add support for custom post types or a mix of any post type.
* Code formatting and inline doc cleanup.
* Use the newer `ignore_sticky_posts` instead of `caller_get_posts`.
* Add `<span>` wrappers for styling the day and comments number.
* Add `.day-duplicate` class to `<li>` if it's a repeating day.
* Add `<div class="clean-my-archives">` wrapper for entire output.

### Version 0.1.0

* Plugin launch.  Everything's new!

## Professional Support

If you need professional plugin support from me, the plugin author, you can access the support forums at [Theme Hybrid](http://themehybrid.com/support), which is a professional WordPress help/support site where I handle support for all my plugins and themes for a community of 40,000+ users (and growing).

## Copyright and License

This project is licensed under the [GNU GPL](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html), version 2 or later.

2008&thinsp;&ndash;&thinsp;2013 &copy; [Justin Tadlock](http://justintadlock.com).