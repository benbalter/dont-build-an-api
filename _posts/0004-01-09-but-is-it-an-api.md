---
title: "But is it **an API**?"
---

## [github.com/benbalter/simple-api](https://github.com/benbalter/simple-api)

{% highlight html %}
<html>
  <body>
    <script src="jquery.min.js"></script>
    <script>
    $.getJSON( "dogs.json", function(dogs) {
      $.each(dogs, function(name, attributes) {
        document.write("<h2>" + name + "</h2>");
        document.write("Age: " + attributes["age"] + "<br />");
        document.write("Breed: " + attributes["breed"] + "<br />");
      });
    })
    </script>
  </body>
</html>
{% endhighlight %}
