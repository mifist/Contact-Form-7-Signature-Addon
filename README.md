Contact Form 7 Signature Addon
==============================

This piece of code is an addon to the famous Contact Form 7 Wordpress plugin.
It brings a new field type to forms that allows users to submit an handwritten signature.

The plugin uses Szymon Nowak's great Javascript library (https://github.com/szimek/signature_pad).

# Installation

This plugin requires the Contact Form 7 plugin.

1. Upload plugin files to your plugins folder, or install using WordPress' built-in Add New Plugin feature
2. Activate the plugin
3. Edit a form in Contact Form 7
4. Choose "Signature field" from the Generate Tag dropdown
5. Follow the instructions on the page

If you want the signature image to be included in the body of your mails, just put an image tag which src attribute is set to the content of your field, like this :
```
<img src="[your-signature-field]"/>
```
Your contact form needs to send **HTML formatted** messages for it to work properly, so don't forget to check the corresponding box at the bottom of your email settings.

[Wordpress plugin repository](http://wordpress.org/plugins/contact-form-7-signature-addon)

# Notes

## Important change since version 2.0
Since version 2.0, the plugin no longer uses inline base64 encoded images, and signature images are saved to a "signatures/" subdir of your wordpress upload directory. So every email clients compatibility issues should be gone !

## CF7 Version compatibility
This plugin was tested with CF7 versions down to 3.5. Use it with older versions at your own risk.
