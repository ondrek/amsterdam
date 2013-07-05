/*
_______________________________
RESET */
*{text-decoration:none;font-size:1em;outline:none;margin:0;padding:0}code,kbd,samp,pre,tt,var,textarea,input,select,isindex,listing,xmp,plaintext{font:inherit;white-space:normal}a,img,a img,iframe,form,abbr,acronym,object,applet,table,a abbr,a acronym{border-width:0}dfn,i,cite,var,address,em{font-style:normal}th,b,strong,h1,h2,h3,h4,h5,h6,dt{font-weight:400}caption,th,td{text-align:left}html{background:#FFF;color:#000;line-height:1;font-family:arial, sans-serif}/* \*/html{font-family:sans-serif}/* */q{quotes:"\201C""\201D""\2018""\2019"}ul,ol,dir, {list-style:none}sub,sup{vertical-align:baseline}a{color:inherit}/*
_______________________________
DISABLE DEPRECATED HTML */
font,basefont{color:inherit;font:inherit;font-size:100%}center,*[align]{text-align:inherit}s,strike,u{text-decoration:inherit}img{border:none;margin:0}ol{list-style-type:decimal}body{background-color:transparent}tr,th,td{width:auto;height:auto;background-color:transparent;vertical-align:inherit;border:none}table[border],.content table[border]{border-collapse:separate;border-spacing:0}nobr{white-space:normal}marquee{overflow:visible;-moz-binding:none}blink{text-decoration:none}/*
_______________________________
GENERAL */
html{font-size:125%}body{font-size:50%}a{text-decoration:underline}strong,th,thead td,h1,h2,h3,h4,h5,h6,dt{font-weight:700}cite,em,dfn{font-style:italic}code,kbd,samp,pre,tt,var,input[type='text'],input[type='password'],textarea{font-size:100%;font-family:mono-space,monospace}pre{white-space:pre}pre *{font-size:100%;white-space:pre}del{text-decoration:line-through}ins,dfn{border-bottom:1px solid #000}small,sup,sub{font-size:85%}big{font-size:125%;line-height:80%}abbr,acronym{text-transform:uppercase;font-size:85%;letter-spacing:.1em}abbr[title],acronym[title],dfn[title]{cursor:help;border-bottom:1px dotted #000}sup{vertical-align:super}sub{vertical-align:sub}blockquote{padding-left:2.2em}hr{display:none/* We will re-reset it later for content */}:lang(af),:lang(nl),:lang(pl){quotes:'\201E' '\201D' '\201A' '\2019'}:lang(bg),:lang(cs),:lang(de),:lang(is),:lang(lt),:lang(sk),:lang(sr),:lang(ro){quotes:'\201E' '\201C' '\201A' '\2018'}:lang(da),:lang(hr){quotes:'\00BB' '\00AB' '\203A' '\2039'}:lang(el),:lang(es),:lang(sq),:lang(tr){quotes:'\00AB' '\00BB' '\2039' '\203A'}:lang(en-GB){quotes:'\2018' '\2019' '\201C' '\201D'}:lang(fi),:lang(sv){quotes:'\201D' '\201D' '\2019' '\2019'}:lang(fr){quotes:'\ab\2005' '\2005\bb' '\2039\2005' '\2005\203a'}*[lang|='en'] q:before{content:'\201C'}*[lang|='en'] q:after{content:'\201D'}*[lang|='en'] q q:before{content:'\2018'}*[lang|='en'] q q:after{content:'\2019'}input,select,button{cursor:pointer}input[type='text'],input[type='password']{cursor:text}input[type='hidden']{display:none}/*
_______________________________
CONTENT */
.content{font-size:1em;line-height:1.4em}.content h1{font-size:1.6em;margin:1em 0 .5em}.content h2{font-size:1.4em;margin:1.07em 0 .535em}.content h3{font-size:1.2em;margin:1.14em 0 .57em}.content h4{font-size:1.0em;margin:1.23em 0 .615em}.content h5{font-size:0.8em;margin:1.33em 0 .67em}.content h6{font-size:0.6em;margin:1.6em 0 .8em}.content hr{display:block;background:#000;color:#000;width:100%;height:1px;border:none}.content ul{list-style:disc outside}.content ol{list-style:decimal outside}.content table{border-collapse:collapse}.content hr,.content p,.content ul,.content ol,.content dl,.content pre,.content address,.content table,.content form{margin-bottom:1.6em}.content p+p{margin-top:-.8em}.content fieldset{margin:1.6em 0;padding:1.6em}/* \*/.content legend{padding-left:.8em;padding-right:.8em}/* *//* for Opera 8 */@media all and min-width 0px{.content legend{margin-bottom:1.6em}.content fieldset{margin-top:0}.content[class^='content'] fieldset{margin-top:1.6em}}.content fieldset>*:first-child{margin-top:0}.content textarea,.content input[type='text']{padding:.1em .2em}.content input{padding:.2em .1em}.content select{padding:.2em .1em 0}.content select[multiple]{margin-bottom:.8em}.content option{padding:0 .4em .1em}.content button{padding:.3em .5em}.content input[type='radio']{position:relative;bottom:-.2em}.content dt{margin-top:.8em;margin-bottom:.4em}.content ul,.content ol{margin-left:2.2em}.content caption,.content form div{padding-bottom:.8em}.content ul ul,content ol ul,.content ul ol,content ol ol{margin-bottom:0}/*
_______________________________
END */

* { font: 15px/1.4em 'Courier New', Courier, monospace !important; }

body {
  color: black;
  font-size: 12px;
  padding: 0;
  margin: 20px;
  width: 640px;  
}

@media only screen and (max-device-width: 480px) {
  body, img, ul, li {
    width: 90% !important;
    height: auto;
    font-size: 85%;
  }
  .pages a {
    margin: 0 0 0 7px !important;
  }
  .blog-info h1  {
    margin: 0 7px 0 0 !important;
  }
  .scriptogram-link {
    bottom: 7px !important;
    right: 5% !important;
  }
}

img {
  display: block;
  margin: 50px 0;
  max-width: 640px;
  height: auto;
}


#menu {
  margin-top: 45px;
  margin-left: 27px;
}

.content hr {
  padding-left: 0 !important;
  background: transparent;
  border-bottom: 1px dashed black;
}

.content p, .content embed, .content pre, .body-post > div:not(.share-buttons), .body-page > div:not(.share-buttons), .content object, .content iframe {
  margin-left: 27px !important;
}

.content pre {
  background: #f5f5f5;
  padding: 13px;
}
.content {
  margin-bottom: 175px;
}

th,b,strong,h1,h2,h3,h4,h5,h6,dt {
  margin-bottom: 20px !important;
  padding: 0;
}

.content h1:before, .content h2:before, .content h3:before, .content h4:before, p.previous-articles:before
{ 
  content:"/* ";
}

.content h1:after, .content h2:after, .content h3:after, .content h4:after, p.previous-articles:after
{ 
  content:" */";
}

.title {
  display: block;
  border-bottom: 4px double black;
  margin: 0;
  margin-bottom: 27px; 
}

.archive-title {
  border-bottom: 1px dashed black;
  padding-bottom: 17px;
  margin-bottom: 35px; 
  font-size: 120%;
  padding-left: 27px;
}

.title h2 {
  margin-top: 0;
}

.date {
  margin-left: 27px;
  margin-bottom: 35px;
  display: block;
  min-width: 1px;
}

.archive-date {
  margin-left: 27px;
  font-size: 120%;
}

a { 
  text-decoration: none;
}


.body-post a, .body-page a
{
  border-bottom: 1px solid grey;
}
.body-post a:after, .body-page a:after
{ 
  font-size: 12px !important;
  font-family: sans-serif;
  content:"\2192";
}

a:hover { 
  border-bottom: 1px solid black;
}



.pages {
  margin-top: -20px;
}
.pages a {
  margin-right: 17px;
}

.container {
  margin: 75px 0 175px 0;
}  

p.previous-articles {
  font-size: 125%;
  margin-bottom: 35px;
}

ul.tags {
  border-top: 1px dashed black;
  margin: 20px 0;
  padding: 20px 0 20px 28px;
}
 
  ul.tags li {
    list-style: none;
    padding: 0;
    margin: 0;
  }
 
    ul.tags li a {
      margin: 0 15px 0 0; 
      float: left; 
      font-family: Helvetica, Arial, sans-serif;
      font-size: 14px;    
    }
 
.share-buttons {
  border-top: 1px dashed black;
  padding: 27px 0 !important;
}

.share-buttons > .share-facebook, .share-buttons > .share-twitter, .share-buttons > .share-gplus {
  opacity: .5;
}


.share-buttons:hover > .share-facebook, .share-buttons:hover > .share-twitter, .share-buttons:hover > .share-gplus {
  opacity: 1
}

.share-twitter, .share-gplus {
  float: left;
  margin-top: 0px;
}
.share-facebook {
  margin-right: 25px;
  float: left;
}

/*
* scriptogr.am link 
* 
* Please do not remove or hide the footer link.
* This link will keep us alive and motivated to continue our service.
*/

.scriptogram-link {
  font-family: sans-serif;
  position: fixed;
	right: 35px;
	bottom: 35px;
	font-size: 9px;
}

  .scriptogram-link a {
    color: #666666;
  }
  

