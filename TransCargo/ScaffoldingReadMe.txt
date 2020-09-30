Support for ASP.NET Core Identity was added to your project.

For setup and configuration information, see https://go.microsoft.com/fwlink/?linkid=2116645.

-------------------------------------------------------
w: 
ul (elementy HTMLa)
dodać:
u-unstyled
-------------------------------------------------------
w:
wwwroot/css/site.css 
zmienić:
a.navbar-brand {
  white-space: normal;
  text-align: center;
  /*word-break: break-all;*/
}
-------------------------------------------------------
w: wwwroot/css/nicepage.css
zmienić:
.u-text {
  /*word-wrap: break-word;*/
  position: relative;
}
-------------------------------------------------------
w: wwwroot/css/{NAZWA_STRONY}.css
zamiana: 
url("~/images/
na:
url("../images/
-------------------------------------------------------
w:  Views/{NAZWA_KONTOLERA}/{NAZWA_STRONY}.cshtml
zmiana:
src="images/
na:
src="~/images/

zamiana:
<link rel="stylesheet" href="~/css/
<script class="u-script" type="text/javascript" src="~/js/jquery.js" defer=""></script>
<script class="u-script" type="text/javascript" src="~/js/nicepage.js" defer=""></script>
    
-------------------------------------------------------

usunąć: wwwroot/js/jquery.js
dalej już nieważne
w: wwwroot/js/jquery.js
zamiana:
/@ ...
na: 
/# sourceMappingURL=jquery.min.map


-------------------------------------------------------
w: wwwroot/js/nicepage.js

zamiana:
.load(f
na:
.on('load', f


zamiana:
.load(u
na:
.on('load', u