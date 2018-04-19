# concrete5_coding_requirements
Lets make concrete5 (marketplace items) great again!

# Themes

## Your theme must:
- be in the package format and install properly for the minimum version of concrete5 as specified in your package controller.
 
- must contain a portable network graphics file (png) named icon.png in your package root. The size of this icon will be 97 pixels square with 4 pixel rounded corners.

- include a portable network graphics file (png) named thumbnail.png, properly sized to an aspect ration of 4 to 3. Keep this file under 360 pixels wide.  It will currently display only at 120 x 90 pixels so excessive width is unnecessary.
 
- display correctly on the Add Functionality page of the concrete5 installation. This can be accomplished with a description.txt file in the theme folder or via the page_theme.php file. Excessively long names or descriptions will be rejected.
 
- use unique file and class handles.

- use snake-case (i.e. "my\_cool\_theme") for naming files and folders. 
 
- contain <?php View::element('header\_required'); ?> anywhere in the head of your theme and <?php View::element('footer\_required'); ?> directly before the </body> tag.

- not change the concrete5 core styling.
 
- have a default.php and view.php. Your view needs to contain this code <?php  print $innerContent; ?> .

- contain a div with the class <?php echo $c->getPageWrapperClass()?> directly after the opening body tag.
  
- comply with all licensing requirements. Include the copyright and licensing information for all js and applicable css files.

- not contain any compiled code.

- output the language of the end users install (i.e. html lang="en").

- not duplicate any code output by the core cms. (e.g. some meta tags are output by the core as is Jquery. Do not duplicate.)

## Your theme should

- use DRY (don't repeat yourself) code.

## Submission Hints

- The Peer Review Board is run by volunteers. Be nice. Say please and thank you. Make changes in a timely fashion. Let us know if you will be unavailable for more than a few days so we know not to delete your submission if we think its abandoned.

- Submit well tested clean code. We don't need extra work.
