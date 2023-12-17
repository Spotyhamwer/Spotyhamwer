- 👋 Hi, I’m @Spotyhamwer
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Spotyhamwer/Spotyhamwer is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<?php
/**
 * Plugin Name: Simple Welcome Widget
 * Description: A simple WordPress plugin that adds a welcome widget to the sidebar.
 * Version: 1.0
 * Author: Your Name
 */

// Exit if accessed directly.
if (!defined('ABSPATH')) {
    exit;
}

// Include the widget class.
include_once(plugin_dir_path(__FILE__) . 'class-simple-welcome-widget.php');

// Register the widget.
function register_simple_welcome_widget() {
    register_widget('Simple_Welcome_Widget');
}
add_action('widgets_init', 'register_simple_welcome_widget');
