# Setting up bootstrap 4 with middleman

1. Install with npm

```
npm install bootstrap@4.0.0-beta 
```

Activate sprockets in `config.rb` and point assets path to `node_modules` with sprockets

```
# Gemfile

gem 'middleman-sprockets', '~> 4.0.0.rc'
```

```
# config.rb

activate :sprockets
sprockets.append_path File.join(root, "node_modules")
```

After that in `application.js` file, add this:

```
//= require bootstrap
```

and `application.scss` add this:

```
@import 'bootstrap';
```

Done!
