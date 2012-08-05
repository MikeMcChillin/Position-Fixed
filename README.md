## This is a CSS trick to reveal content on page scroll.

It produces a nice revealing "wipe" effect on the page, giving the illusion that some content is on top of other content... because technically it is.
This trick utilizes position: fixed; and z-index; on the content you'd like to "wipe" over.

#Essential CSS elements:
* { margin: 0; padding: 0;}
html,body { height: 100%;}
body { width: 100%;}
header { position: fixed; top: 0; left: 0; width: 100%; z-index: 1; }
.browser-height { height: 100%;}
.main { position: relative; height: 1200px; background: #F72E2A; z-index: 3; margin:0; padding: 0; box-shadow: 0 0 3px #333; }
.footer-wrap { background: purple url('http://25.media.tumblr.com/tumblr_m457hiwVq61qea3oqo1_1280.jpg') no-repeat fixed bottom center; background-size: 100%; position: relative; z-index: 2; width: 100%; height: 100%; }

Demo here: http://mcchill.in/lab/positionfixed/index.html