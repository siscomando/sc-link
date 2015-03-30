sc-link
=======

The sc-link to fire an custom event, open (or not) links in href attributes.

Usage
=====

```
<body unresolved>

      <sc-link href="http://hipy.co" eventname="sc-select" continue="true">
        2015RI/00000345
      </sc-link>

      <script>
        window.addEventListener('polymer-ready', function(e) {
          var link = document.querySelector('sc-link');
          link.addEventListener('sc-select', function(e) {
            console.log(e.detail.issue);
          });
        });
      </script>
</body>
```
