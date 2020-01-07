<h1>Boostrap 4 Lightbox gallery using JQuery</h1>
<h1>Getting Started</h1>
<p>In this tutorial We have create lightbox gallery using JQuery. We have to use ekko-lightbox library files for the lightbox gallery.</p>
<h1>Installation & Usage:</h1>
<ol><li>In your<code>&lt;head&gt;</code>section, add the following <em>stylesheet</em> links</li></ol>
<pre><code>  &lt;link href="https://cdnjs.cloudflare.com/ajax/libs/ekko-lightbox/5.3.0/ekko-lightbox.css" rel="stylesheet"&gt;</code></pre>
<ol start="2"><li>Before the end of your<code>&lt;body&gt;</code>section, add the following <em>javascript</em> links. This library depends on jQuery, so jQuery must also be included, before these scripts are run</li></ol>
<pre><code>  &lt;script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"&gt;&lt;/script&gt;
  &lt;script src="https://cdnjs.cloudflare.com/ajax/libs/ekko-lightbox/5.3.0/ekko-lightbox.js"&gt;&lt;/script&gt;
  &lt;script src="https://cdnjs.cloudflare.com/ajax/libs/ekko-lightbox/5.3.0/ekko-lightbox.js.map"&gt;&lt;/script&gt;
  &lt;script src="https://cdnjs.cloudflare.com/ajax/libs/ekko-lightbox/5.3.0/ekko-lightbox.min.js"&gt;&lt;/script&gt;
  &lt;script src="https://cdnjs.cloudflare.com/ajax/libs/ekko-lightbox/5.3.0/ekko-lightbox.min.js.map"&gt;&lt;/script&gt;
</code></pre>
<ol start="3"><li>Add the images in the <code>&lt;body&gt;</code> section.</li></ol>
<pre><code>&lt;a href="images/image-1.jpg" data-toogle="lightbox" data-gallery="gallery" class="col-md-3"&gt;
  &lt;img src="images/image-1.jpg" class="img-fluid" &gt;
&lt;/a&gt;</code></pre>
<ol start="4"><li>Add this <code>&lt;script&gt;</code>function before the close <code>&lt;body&gt;</code>section.</li></ol>
<pre><code>&lt;script type="text/javascript"&gt;
  $(document).on("click", '[data-toggle="lightbox"]', function(event) {
    event.preventDefault();
    $(this).ekkoLightbox();
  });
&lt;/script&gt;</code></pre>
