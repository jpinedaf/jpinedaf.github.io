---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: photo_mobile.jpg
widget1:
  title: "About"
  url: '/info/'
  image: photo.jpg
  text: 'Learn more about my work as a Staff Astronomer at the Max Planck Institute for Extraterrestrial Physics and my research interests in star formation and gas kinematics.'
widget2:
  title: "Research"
  url: '/research/'
  text: 'Explore current projects and selected publications on molecular clouds, star and disk formation, and astrochemical approaches to gas kinematics.'
  image: B5_transition_to_coherence.jpg
widget3:
  title: "CV"
  url: '/cv/'
  image: B5_filament_fragmentation.jpg
  text: 'Find a summary of appointments and education, and download the full CV.'
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: /contact/
  text: Contact Jaime Pineda ›
  style: success
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---
