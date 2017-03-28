---
title: Configuration and Hooks
table_of_contents: true
---

# Configuration and hooks

``` yaml
hooks: # Top-level YAML attribute, parallel to `apps`
    upgrade: # Hook name, corresponds to executable name
        plugs: [network] # Or any other plugs required by this hook
```

``` python
from fish.chips import MyLunch

# A python comment

class SomeClass:
  arg_one: "hello"

  def a_method(argument, argument2=value):
    """
    Docstring
    """

    variable = "string"
    another = 123

    if some_condition >= 20 and x == y:
      print "go away"

    return HELLO_WORLD
```

``` markdown
# Hello

A line with [a link](http://somewhere.com).

Top level 2
===

a [nother link][nother], *this* time with **reference** style.

## Second level heading

### Third level heading

Second level again
---

#### Fourth

---

[nother]: http://example.com "An example link"

```

``` html
<!doctype html>

<html>
  <body>
    <!-- example document -->
    <script>
      document.write('hello world');
    </script>
    <style>
      h1 {font-weight: bold;}
    </style>
    <div class="highlighter-rouge">
      <h1>First heading</h1>
      <p>Hello&nbsp;world</p>
      <h2>Second heading</h2>
      <br/>
      <pre class="highlight">
        <code>
          <!-- Code -->
        </code>
      </pre>
    </div>
  </body>
</html>
```

``` JavaScript
/**
 * Multiline comment
 * line two
 */
function Point(x, y) {
    this.x = x;
    this.y = y;

    // Normal comment
}
Point.prototype = {
    dist: function () {
        return Math.sqrt((this.x*this.x)+(this.y*this.y));
    },
    toString: function () {
        return "("+this.x+", "+this.y+")";
    }
}
```

``` bash
$ sudo apt-get install mysql-server libapache2-mod-auth-mysql php5-mysql
$ ifconfig eth0 | grep inet | awk '{ print $2 }'
By default, a MySQL installation has an anonymous user, allowing anyone
to log into MySQL without having to have a user account created for
them.  This is intended only for testing, and to make the installation
go a bit smoother.  You should remove them before moving into a
production environment.

Remove anonymous users? [Y/n] y                                            
 ... Success!
```

``` sass
// Footer pattern styling
@mixin vf-p-footer {

  .p-footer {
    border-top: 1px dotted $color-x-dark;
    font-size: .75rem;
    margin-bottom: 1rem;
    padding-top: .75rem;

    @media (min-width: $breakpoint-medium) {
      font-size: .8125rem;
    }

    &__copy {
      margin-bottom: 0;
    }

    &__links {
      margin: 0;
      padding: .5rem 0;

      @media (min-width: $breakpoint-medium) {
        margin-top: 0;
        padding: 0;
      }
    }
```

```bash
#!/bin/sh

# optionally set the url of the service
snapctl set device-service.url="https://device-service"
# set optional extra HTTP headers for requests to the service
snapctl set device-service.headers='{"token": "TOKEN"}'

# set an optional proposed serial identifier, depending on the service
# this can end up being ignored;
# this might need to be obtained dynamically
snapctl set registration.proposed-serial="DEVICE-SERIAL"

# optionally pass details of the device as the body of registration request,
# the body is text, typically YAML;
# this might need to be obtained dynamically
snapctl set registration.body='mac: "00:00:00:00:ff:00"'

```
