<h3 id='res.links'>res.links(links)</h3>

Join the given `links` to populate the "Link" response header field.

{% highlight js %}
res.links({
  next: 'http://api.example.com/users?page=2',
  last: 'http://api.example.com/users?page=5'
});
{% endhighlight %}

p yields:

{% highlight js %}
Link: &lt;http://api.example.com/users?page=2&gt;; rel="next",
      &lt;http://api.example.com/users?page=5&gt;; rel="last"
{% endhighlight %}
