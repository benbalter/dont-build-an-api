---
title: An example **Build Script**
---

{% highlight ruby linenos %}
require 'csv'
require 'json'

CSV.foreach( "./data/puppies.csv", :headers => true ) do |puppy|
  File.open( "./api/#{puppy[:name].downcase}.json", 'w') do |file|
    file.write puppy.to_json
  end
end
{% endhighlight %}
