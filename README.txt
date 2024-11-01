=== Plugin Name ===
Contributors: multimedianj
Tags: a11y, accessibility, accessible, wcag, web accessibility, navigation, toolbar, sidebar
Requires at least: 4.9
Tested up to: 5.8.2
Stable tag: 1.1.0
Requires PHP: 7.2
License: GPLv3

Make your website accessibility better by adding pre-configured and custom settings in your menu.

== Description ==

This plugin offers you the possibility to show people accessibility configurations in your menu. This means that everyone, including people with disabilities, will be able to configure the settings (contrast, font-size, coloration, ...) that help them be able to use your website.

Here is a [demo](https://demo.wpinclusion.com/a11y-kit).
Follow the evolution of the plugin trough the [Github repository](https://github.com/multimedianj/a11y-kit).

In order to make the plugin works, you need to create a menu first.
In your menu, you simply need to add a CSS class in this way **"wpak_DISABILITY_PROPERTY"**.

Where to add the CSS class mentioned above ?
- In the menu you're in (Appearance > Menus > name_of_your_menu), you first click on an item you want to have the ability to change the state (accessibility menu item).
- Then, you should have the field "CSS Classes (optional)". Inside this field, you can add the class in this way : **"wpak_DISABILITY_PROPERTY"** (see examples from the pre-configured classes below).
- If the field "CSS Classes (optional)" is not visible, you just have to look for the "Screen Options" button in the top-right corner of the page. Then, search for the checkbox "CSS Classes" which should be checked in order for the field to be visible. Finally, return to the field and add your class.

### List of the pre-configured classes
= Coloration =
- "wpak_color_normal" (normal state)
- "wpak_color_dark" (dark mode)
- "wpak_color_monochrome" (shades of gray, monochrome)
- "wpak_color_highcontrast" (high contrast)
- "wpak_color_lowsaturation" (low saturation)
- "wpak_color_highsaturation" (high saturation)

= Font size =
- "wpak_font_normal" (normal state)
- "wpak_font_large" (large font-size, default: 30px)

= Dyslexia =
- "wpak_dyslexia_normal" (normal state)
- "wpak_dyslexia_comicsans" (Comic Sans font-family)
- "wpak_dyslexia_arial" (Arial font-family)

= Reset button =
- "wpakReset" (reset all the filters)

### Add an icon instead of text
You can use the field for the title to add HTML code. With HTML code, it is possible to add
- An image: `<img src="link_of_your_image.png" alt="name_of_property" />`
- An icon from FontAwesome or any library you want to include: `<i class="fas fa-adjust"></i>`

###  Suggested FontAwesome icons
Here is a list of the suggested icons to use for each pre-configured accessibility settings.

- Coloration: `<i class="fas fa-adjust" title="Change the coloration of the site"></i>`
- Font-size: `<i class="fas fa-font" title="Change the font-size of the site"></i>`
- Font-family: `<i class="fas fa-pencil-alt" title="Change the font-family of the site"></i>`
- Letter-spacing: `<i class="fas fa-text-width" title="Change the letter-spacing of the site"></i>`
- Line-height: `<i class="fas fa-text-height" title="Change the line-height of the site"></i>`
- Reset button: `<i class="fas fa-undo" title="Reset all the accessibility configurations"></i>`

= EXTRA =
If you want to add a link to your accessibility statement page, we recommend using this icon that displays perfectly
- `<i class="fas fa-child" title="Go to the accessibility statement page"></i>`

###  Import a pre-generated menu
To import a pre-generated menu with already pre-configured accessibility settings, follow the instructions below.

1. First, download the file **menu-a11y.json** on your computer, available in the folder **SAMPLE** of the plugin
1. Install the plugin **Export Import Menus", available [here](https://wordpress.org/plugins/export-import-menus)
1. Activate the plugin
1. Go to **Appearance > Export/Import Menus**
1. Click on the tab **Import Menus**
1. Click on **Choose a file** and import the **menu-a11y.json** file you just downloaded on your computer
1. On the **Menu Name** field, feel free to name your menu (ex.: A11y topbar menu)
1. Click on the **Import Menus** button
1. Validate in **Appearance > Menus** that your menu has been imported correctly

= EXTRA =
If you want to use FontAwesome icons, install the plugin FontAwesome, available [here](https://wordpress.org/plugins/font-awesome)

###  Overwritte accessibility settings (styles)
In the plugin directory, there's a file **SAMPLE/style-a11y.css** that contains all the CSS variables used to style the different accessibility settings of the plugin. It is possible to overwritte those variables by adding this file to the root of your theme.

1. You need to download the **style-a11y.css**
1. You add the file to the root of your theme (or child-theme)
1. You add this code to your style.css **@import "style-a11y.css";**

This plugin was created and is maintained by WP inclusion, a [glossary of Web accessibility terminologies](https://wpinclusion.com).

### Compatibility

This plugin is multilingual ready.


== Installation ==

This section describes how to install the plugin and get it working.

e.g.

1. Upload `a11y-kit.zip` to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress
1. You need to create a menu in order for the plugin to work.
1. The trick is to simply add a CSS class in this way "wpak_DISABILITY_PROPERTY" in order to add custom styles to your accessibility settings.


== Changelog ==

= 1.1.0 =
* Fix bug on plugin removal (deletion)
* Improve documentation (instructions) on how to configure the accessibility menu

= 1.0.1 =
* Add a DEMO (URL link) of the plugin to better understand the final result

= 1.0.0 =
* Fix the problem of displaying the documentation to WordPress.org

= 0.0.3 =
* Export pre-generated menu in JSON file and add it as a SAMPLE
* Documentation to import a pre-generated menu with FontAwesome icons

= 0.0.2 =
* Add a better documentation to the usability of the plugin
* Update the "dark mode" styles
* Update the "high contrast" styles

= 0.0.1 =
* Initial commit
