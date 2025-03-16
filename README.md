OpenRouter Chat Plugin for WordPress

Overview
The OpenRouter Chat Plugin integrates the OpenRouter API with your WordPress site, 
allowing users to interact with AI models like Qwen (qwen/qwq-32b:free) through a chat interface. 
The plugin provides a shortcode [openrouter_chat] to embed the chat functionality 
anywhere on your site, such as posts, pages, or widgets.

This plugin is ideal for adding an interactive AI-powered chatbot to your WordPress site, 
enhancing user engagement and providing dynamic content.

Features

AI-Powered Chat : Communicate with the Qwen model via the OpenRouter API.
Shortcode Support : Embed the chat interface using the [openrouter_chat] shortcode.
Dark Theme : Stylish dark-themed design for a modern look.
Retry Logic : Automatically retries failed API requests up to 3 times.
Secure API Key Storage : Store your OpenRouter API key securely in the WordPress admin settings.
AJAX-Based Communication : Smooth and asynchronous interaction without page reloads.
Error Handling : Gracefully handles errors and timeouts with user-friendly messages.

Installation

Step 1: Upload the Plugin
Download the plugin files and extract them.
Upload the peepso-openrouter-chat folder to your WordPress plugins directory
wp-content/plugins/

Step 2: Activate the Plugin
Log in to your WordPress admin dashboard.
Navigate to Plugins > Installed Plugins .
Locate OpenRouter Chat Plugin in the list and click Activate .

Configuration

Step 1: Add Your OpenRouter API Key
Go to Settings > OpenRouter Chat in your WordPress admin dashboard.
Enter your OpenRouter API key in the provided field.
Click Save Changes .
Note : You can obtain your API key by signing up at OpenRouter . 

Step 2: Use the Shortcode
To display the chat interface, use the [openrouter_chat] shortcode in any post, page, or widget:


Copy
[openrouter_chat]

Usage

After activating the plugin and configuring your API key, add the [openrouter_chat] shortcode to any page or post.
Visit the page where the shortcode is embedded.
Type a message in the input field and click Send to interact with the AI model.

Customization

Dark Theme
The plugin includes a sleek dark theme by default. If you'd like to customize the colors or styles:

Edit the CSS file located at:

assets/css/style.css
Update the styles as needed and save the file.

Troubleshooting

Common Issues and Solutions
Chat Not Working :
Ensure your OpenRouter API key is correctly configured in Settings > OpenRouter Chat .
Check the browser console for JavaScript errors and ensure the AJAX request is being sent.
Timeout Errors :

If you encounter timeout errors, ensure your server has sufficient resources and network connectivity.
The plugin includes retry logic, but you can increase the timeout further if needed (see timeout in the code).
Unexpected API Response :
Verify that the model ID (qwen/qwq-32b:free) is correct and supported by OpenRouter.
Check the debug.log file for detailed API response logs.

Critical Errors :

Enable debugging in WordPress by adding the following lines to your wp-config.php file:
php

define('WP_DEBUG', true);
define('WP_DEBUG_LOG', true);
define('WP_DEBUG_DISPLAY', false);
Review the wp-content/debug.log file for error details.
Support
If you encounter any issues or have questions about the plugin, feel free to reach out:


Email : dakota@contentsocial.net

Changelog
Version 1.0
Initial release of the OpenRouter Chat Plugin.
Added support for the Qwen model (qwen/qwq-32b:free).
Included a shortcode [openrouter_chat] for embedding the chat interface.
Styled the chat interface with a dark theme.
Implemented retry logic and error handling for robust communication with the OpenRouter API.

License
This plugin is released under the GNU General Public License v2 or later (GPL-2.0-or-later) . 
You are free to use, modify, and distribute this plugin as long as you adhere to the terms of the license.

Thank you for using the OpenRouter Chat Plugin! We hope it enhances your WordPress site and provides a seamless 
AI-powered chat experience for your users. If you find this plugin helpful, please consider leaving a review

