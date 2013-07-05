<!DOCTYPE html> 
<html lang="en"><head>

	<meta charset="utf-8" />

	<title>{{author}}{{#is_post}}{{#posts}} | {{title}}{{/posts}}{{/is_post}}{{#is_page}}{{#posts}} | {{title}}{{/posts}}{{/is_page}}</title>

	<meta name="description" content="{{author}} {{blog_title}}" />

	<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
	<meta http-equiv="X-UA-Compatible" content="IE=edge" />

	<meta name="description" content="{{author}} | {{blog_title}}" />
	<meta name="robots" content="index, follow" />

	<link rel="shortcut icon" href="http://scriptogr.am/lib/img/favicon.ico" />
	<link rel="alternate" type="application/rss+xml" title="RSS" href="{{base_url}}/feed" />

	{{css}}

</head><body>

	<header>
		<h1><a href="{{home_link}}">{{author}}'s Blog</a></h1>
		<h2>{{blog_title}}</h2>
	</header>

	<nav>
		{{#pages}}
		<a href="{{permalink}}">#{{title}}</a>
		{{/pages}}
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

		{{#is_post}}

			<article>
		
				<time>{{prettydate}}</time>
				<h2><a href="{{permalink}}">{{title}}</a> {{#post_permalink}}<a href="{{post_permalink}}">#</a>{{/post_permalink}}</h2>
		
				{{#excerpt}}<span class="introduction">{{excerpt}}</span>{{/excerpt}}
		
				{{content}}
		
				{{#if_tags}}
				<ul class="tags">
				{{#tags}}
				<li><a href="{{base_url}}/tag/{{name}}">{{name}}</a></li>
				{{/tags}}
				</ul>  
				{{/if_tags}}
		
				<a href="{{home_link}}/archive">More articles</a>
		
			</article>

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

	<footer>
		Using <a href="http://scriptogr.am">Scriptogr.am</a>, Semantical HTML5 markup &amp; Dropbox
	</footer>

	<!-- this is way how to disable scriptogram google analytics - bit.ly/13qdiuX & bit.ly/19ZG5p3 -->
	<script>window['ga-disable-UA-33446752-1'] = true;</script>
	
</body></html>                                                                                                                                                                                                                                                                                                                                                     
