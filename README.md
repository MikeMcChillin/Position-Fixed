# This is a CSS trick to reveal content on page scroll.

It produces a nice revealing "wipe" effect on the page, giving the illusion that some content is on top of other content... because technically it is.
This trick utilizes position: fixed; and z-index; on the content you'd like to "wipe" over.

##Essential CSS elements:
	* { margin: 0; padding: 0;}
	html,body { height: 100%;}
	body { width: 100%;}
	header { position: fixed; top: 0; left: 0; width: 100%; z-index: 1; }
	.browser-height { height: 67%;}
	.main { position: relative;  background: #f0f0f0; z-index: 3; margin:0; padding: 0; box-shadow: 0 0 10px 0 rgba(0, 0, 0, .7); }
	.footer-wrap { background: #fff; position: relative; z-index: 2; width: 100%; height: 260px;}

Demo here: http://mcchill.in/lab/positionfixed/index.html