=== Search Exclude ===
Contributors: Komal Bhatt
Tags: search, exclude, posts, pages, custom post types
Requires at least: 5.5
Tested up to: 6.7
Stable tag: 1.0.0
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Exclude specific pages, posts, and custom post types from WordPress search results.

== Description ==

**Search Exclude** gives you a clean, easy-to-use admin interface to control exactly what appears in your WordPress search results:

* **Exclude individual posts/pages/CPTs** – Live search for any content and add it to the exclusion list with one click.
* **Exclude entire post types** – Toggle off whole post types (e.g. WooCommerce Products, Events, etc.) from search results.
* Works with any registered public post type.
* Lightweight — uses a single `pre_get_posts` filter, no database bloat.

== Installation ==

1. Upload the `search-exclude` folder to `/wp-content/plugins/`.
2. Activate the plugin from the **Plugins** menu in WordPress.
3. Navigate to **Settings → Search Exclude** to configure.

== Steps to be followed ==
To EXCLUDE a page from search:
1. Go to Settings → Search Exclude
2. Search for the page and click + Add
3. Click Save & Sync to Algolia
4. Click Force Sync Now
✅ Page is removed from Algolia search
To RESTORE a page back to search:
1. Go to Settings → Search Exclude
2. Click ✕ to remove the page from the exclusion list
3. Click Save & Sync to Algolia
4. Run full re-index from your Algolia plugin
5. Click Force Sync Now (to re-exclude any other pages still on the list)
✅ Page is back in Algolia search
Golden rule → always end with Force Sync Now after any re-index.

== Changelog ==

= 1.0.0 =
* Initial release.
