=== TS Contact Form ===

Plugin Name: TS Contact Form
Plugin URI: www.tatianadeaguiar.com.br
Description: A clean, secure, and easy-to-use contact form plugin for WordPress.
Tags: contact, form, contact form, email, mail, captcha
Author: Tatiana Scheidegger de Aguiar Alves
Author URI: not available
Donate Link: #
Requires at least: 4.0
Tested up to: 4.3
Stable Tag: trunk
Version: 20150808
Text Domain: scf
Domain Path: /languages/
License: GPL v2 or later

TS Contact Form is a simple, secure, and easy-to-use contact form plugin for WordPress.

== Description ==

[TS Contact Form]

Overview

Easy Setup: Use shortcode or template tag to display the form anywhere on your site.
Well-Formatted Emails: TS Contact Form sends descriptive and well-formatted email messages in plain text.
Secure: Blocks spam and protects against malicious content.
Clean Code: Lightweight, standards-compliant, semantic, and valid markup.
Fully Customizable: Easily configure and style from the Settings page.
Features

User-friendly Settings Page with a toggling panel for easy customization.
Style the form via the Settings Page with your own custom CSS.
Template tag to display TS Contact Form anywhere in your theme.
Shortcode to display TS Contact Form on any post or page.
Customizable confirmation message for the sender.
Customizable placeholder text for input fields.
Option to use PHP’s mail() or WP’s wp_mail() (default).
Option to display message only in the success message.
Anti-Spam & Security

Captcha: Includes challenge question/answer (with option to disable for users).
Firewall: Secure form processing protects against bots and malicious input.
User-friendly: Same-page error messages to help users complete required fields.
Clean Code

Immaculate PHP: Every line is meticulously crafted.
Clean Markup: Well-formatted source code with proper alignment and spacing.
Well-Formatted Emails: Delivered emails present descriptive and well-structured content.
Improved Performance: Custom CSS styles load only where the contact form is displayed.
More Features

Functions perfectly without JavaScript.
Option to reset default settings.
Customization options for various aspects of the form.
Customizable success, error, and spam messages.
Option to enable or disable CSS styles.
Email message includes IP, host, agent, and other user details.
Customizable form field labels, error messages, and success messages.
== Installation ==

Installation

Typical plugin install: Upload, activate, and customize in WP Admin.

Unzip and upload the entire directory to your "plugins" folder and activate.
Use the shortcode to display TS Contact Form on any post or page, or:
Use the template tag to display TS Contact Form anywhere in your theme.
Visit the TS Contact Form Settings Page to configure your options and for more information.
Usage: Visit the plugin’s settings page for shortcodes, template tags, and more information.

Shortcode

csharp
[simple_contact_form]
Template Tag

php
<?php if (function_exists('simple_contact_form')) simple_contact_form(); ?>
== Upgrade Notice ==

To upgrade the plugin, remove the old version and replace it with the new version. Nothing else needs to be done.

== Changelog ==

20150808

Tested on WordPress 4.3
Updated minimum version requirement
20150507

Tested with WP 4.2 + 4.3 (alpha)
Changed some "http" links to "https"
Added Dutch translation; thanks to Martijn van Es
Bugfix: HTML attributes were being stripped from custom error messages
20150317

New! Added subject field to the form
Tested with the latest WP version (4.1)
Increased minimum version to WP 3.8
Removed deprecated screen_icon()
Added $scf_wp_vers for version check
Added UTF-8 as default for WP option used in htmlentities()
Replaced sanitize_text_field() and filter_var() with sanitize_email() for email addresses
Streamlined/fine-tuned plugin code
Added nonce security to the form
Localized some missing strings
Added Reply-To and Return-Path to email headers
Added Text Domain and Domain Path to file header
Replaced default .mo/.po templates with .pot template
20140925

Tested on the latest WordPress version (4.0)
Increased minimum required version to WP 3.7
Added conditional check to min-version function
Reorganized the plugin settings page
Added .scf class to both form div and success div
Added scf_filter_contact_form filter to form output
Fixed case-sensitivity bug for challenge question
Replaced 'UTF-8' with get_option('blog_charset') in scf_process_contact_form()
Replaced stripslashes(), htmlentities(), filter_var() with sanitize_text_field()
Fixed weird character and backslash issues (related)
Applied i18n to email content and success message
Generated new mo/po translation files
20140305

Added default templates for translation/localization
Added language support for Spanish
Changed default option for Time Offset
20140123

Tested with latest WordPress (3.8)
Added trailing slash to load_plugin_textdomain()
Fixed 3 incorrect _e() tags in core file
Localized default options
20131107

Renamed add_plugin_links to add_scf_links
Revised "Welcome" panel in plugin settings
20131106

Added option to hide extra information displayed in the success message
Fixed logic for using mail() vs wp_mail()
Removed "Δ" from die() for better security
Added i18n/localization support
Added "rate this plugin" links
Added uninstall.php file
Added parameters to htmlentities (fixes weird characters issue)
Replaced get_permalink() with an empty value in the form
Changed $date to use WordPress settings and format
Fixed character encoding via filter_var and html_entity_decode in scf_process_contact_form()
Tested on latest WordPress version (3.7)
General code cleanup and maintenance
Version 20130725

Tightened form security
Tightened plugin security
Version 20130712

Fixed time offset setting
Defined UTC as default time
Improved localization support
Replaced deprecated functions
Added options to customize placeholder text for form inputs
Added option to use either PHP's mail() or WP's wp_mail() (default)
Overview and Updates panels now toggled open by default
General code check and clean
Version 20130104

"Send email" (submit) button now available for translation
Added option to disable the Captcha (challenge question/response)
Added option to disable the automatic carbon copy
Added margin to submit button (required in 3.5)
Fixed "Undefined index" warning
Version 20121205

Now hides unsightly fieldset borders by default
Errors now include placeholder attributes
Anti-spam placeholder now displays challenge question
Removed blank line from successful message results
Markup can now be used in custom prepend/append content
Custom CSS now loads on successful result output
Wrapped successful result output with div #scf_success
Segregated custom content for form and success results
Cleaned up some code formatting
Moved .clear div to optional custom content
Added link to TS Contact Form CSS Hooks in Appearance options
Fixed the plugin’s built-in time offset
Version 20121103

Initial release.