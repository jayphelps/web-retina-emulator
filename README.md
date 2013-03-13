WRE (Web Retina Emulator)
=========================

For anyone who has a normal 72/96 dpi display but wants to get a "glance" at how their HTML is rendering for retina displays. It will basically just make your page twice as big, allowing you to quickly see what images are not retina-ready and also point out any CSS properties that may cause blurriness. (like 3d transforms)


Bookmarklet
-----------

To use it as a bookmarklet, just prefix the code with "javascript:".

Known Issues
------------

  * Fixed positioned elements may shift in WebKit browsers because of issues with position: fixed; and -webkit-transform's. WebKit has been fixed but the patch hasn't made it into any Chrome/Safari release yet.
  * Firefox doesn't allow JavaScript that was copy-pasted in the URL to have access to most things so this script can't run. Use a bookmarklet instead.
  * Doesn't trigger CSS media queries that that use device pixel ratio/min-resolution; so if you use these you'll need to temporarily adjust them. (Pull request anyone?)
