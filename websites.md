---
layout: default
comments: true
---
### Best Islamic websites
The following are a list of best islamic websites.

|#|Logo|Website|Description|
|-|-|-|-|
{% for website in site.data.websites %}|{{website.id}}|[![{{website.websitename}}]({{website.imagelink}}){: height="150" width="150" .img-responsive .img-thumbnail}]({{website.link}})| {{website.websitename}} |{{ website.description | markdownify_ }}|
{% endfor %}{: .table .table-striped .table-hover}

{% if page.comments %}
<div id="disqus_thread"></div>
<script>
/**
* RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
* LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables
*/
/*
var disqus_config = function () {
this.page.url = http://alreem.github.io/islamic-apps/; // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};
*/
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');

s.src = '//islamic-apps.disqus.com/embed.js';

s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript" rel="nofollow">comments powered by Disqus.</a></noscript>
{% endif %}
