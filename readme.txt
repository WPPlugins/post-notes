=== Post Notes ===
Contributors: jchristopher
Tags: post, posts, notes, wysiwyg
Requires at least: 2.7
Tested up to: 2.7
Stable tag: 1.0

Provides ability to add any number of WYSIWYG formatted notes to each post

== Description ==

Provides ability to add any number of WYSIWYG formatted notes to each post.

View more details as well as a screencast at [the official Plugin page](http://mondaybynoon.com/wordpress-post-notes/ "WordPress Post Notes Official plugin page")

Compatible with WordPress 2.7

== Installation ==

1. Download the plugin and unzip it into your /wp-content/plugins/ directory.
2. Activate the plugin through the 'Plugins' admin menu in WordPress

To retrieve an associative array containing all Notes for a post, use the following within The Loop:	

`<?php $post_notes = post_notes_get_notes(); ?>`

You will be provided an associative array with which to work in your template:

`<?php $total_notes = sizeof($post_notes); ?>
<?php if($total_notes>0) : ?>
	<?php for ($i = 0; $i < $total_notes; $i++) : ?>
		<div class="post-note">
			<div><?php echo $total_notes[$i]['text']; ?></div>
		</div>
	<?php endfor ?>
<?php endif ?>`

== Screenshots ==

1. Post Note