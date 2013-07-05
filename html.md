<!DOCTYPE html> 
<html lang="en"><head>

	<meta charset="utf-8" />

	<title>{{author}}{{#is_post}}{{#posts}} | {{title}}{{/posts}}{{/is_post}}{{#is_page}}{{#posts}} | {{title}}{{/posts}}{{/is_page}}</title>
	
	<meta name="description" content="{{author}} {{blog_title}}" />
	<meta name="viewport" content="width=device-width; initial-scale=1.0; maximum-scale=1.0;" />
	<meta name="apple-mobile-web-app-capable" content="yes" />
	
	<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
	<meta http-equiv="X-UA-Compatible" content="IE=edge" />

	<meta name="description" content="{{author}} | {{blog_title}}" />
	<meta name="robots" content="index, follow" />

	<meta property="og:url" content="{{home_link}}" />
	<meta property="og:site_name" content="{{author}} on scriptogr.am" />

	<link rel="shortcut icon" href="http://scriptogr.am/lib/img/favicon.ico" />
	<link rel="alternate" type="application/rss+xml" title="RSS" href="{{base_url}}/feed" />

	{{css}}

</head><body>
	
	<header>
		<h1><a href="{{home_link}}">{{author}}'s Blog</a></h1>
		<h2>{{blog_title}}</h2>
	</header>

	<nav>
		<ul>
			{{#pages}}
			<li><a href="{{permalink}}">#{{title}}</a></li>
			{{/pages}}
		</ul>
	</nav>
	
	{{#is_index}}

		<ul>
		{{#posts}}
	
			<li>
				<time>{{prettydate}}</time>
				<h3><a href="{{permalink}}">{{title}}</a></h3>
			</li>
	
		{{/posts}} 
		</ul>
		
		{{pagination}}

	{{/is_index}}
	
	{{#is_archive}}

		<ul>
		{{#posts}}
	
			<li>
				<time>{{prettydate}}</time>
				<h3><a href="{{permalink}}">{{title}}</a></h3>
			</li>
	
		{{/posts}} 
		</ul>

	{{/is_archive}}
	
	
	
	{{#posts}}
	
	<article>
	
	
		{{#is_post}}
	
			<div class="post">
			<div class="content">
			<div class="date">{{prettydate}}</div>
			<div class="title"><h2><a href="{{permalink}}">{{title}}</a> {{#post_permalink}}<a href="{{post_permalink}}">#</a>{{/post_permalink}}</h2></div>
			<div class="body-post">
			<!--if excerpt-->
			{{#excerpt}}<span class="introduction">{{excerpt}}</span>{{/excerpt}}
			<!--endif-->
			{{content}}
			<!-- if tags -->
			{{#if_tags}}
			<ul class="tags">
			{{#tags}}
			<li><a href="{{base_url}}/tag/{{name}}">{{name}}</a></li>
			{{/tags}}
			</ul>  
			{{/if_tags}}
			<!-- endif -->
			<!-- social buttons -->
			<div class="share-buttons">
			<div class="share-twitter">
			<a href="https://twitter.com/share" class="twitter-share-button" data-url="{{permalink}}" data-via="scriptogram">Tweet</a><script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src="//platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");</script>             
			</div>
			<div class="share-facebook">
			<div class="fb-like" data-href="{{permalink}}" data-send="false" data-layout="button_count" data-width="50" data-show-faces="false" data-font="arial"></div>
			</div>
			<div class="share-gplus">
			<g:plusone size="medium" href="{{permalink}}"></g:plusone>
			</div>
			</div>
			</div><!--end body-->
			</div><!--end content-->
			<div class="clear"></div>
			</div><!--end post-->          
			<p class="previous-articles"><a href="{{home_link}}/archive">More articles</p>
	
		{{/is_post}}
	

	
		{{#is_page}}
		
			<section>
				
				<h2>
					<a href="{{permalink}}">{{title}}</a>
					{{#post_permalink}} 
					<a href="{{post_permalink}}">#</a>
					{{/post_permalink}}
				</h2>
				
				{{#excerpt}}
					<p>{{excerpt}}</p>
				{{/excerpt}}
				
				<p>{{content}}</p>
				
				{{#if_tags}}
					<ul class="tags">
						{{#tags}}
							<li><a href="{{base_url}}/tag/{{name}}">{{name}}</a></li>
						{{/tags}}
					</ul>  
				{{/if_tags}}
				
			</section>
	
		{{/is_page}}

	{{/posts}} 

	

	</article>

	<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.6.1/jquery.min.js"></script>

</body></html>                                                                                                                                                                                                                                                                                                                                                     
