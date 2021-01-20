My personal website where I talk about web, and mobile development.

## How it works?

I use [Jekyll](http://jekyllrb.com/), a static generator in Ruby, to create this blog.

## First steps

1. Install [Git](http://git-scm.com/downloads) and [Ruby](http://www.ruby-lang.org/pt/downloads/), in case you don't have them yet.

2. Once installed these dependencies, open up the terminal and install [Jekyll](http://jekyllrb.com/) with the following command:

  ```sh
  $ gem install jekyll
  ```

3. Now clone the project:

  ```sh
  $ git clone git@github.com:thamaraaalves/thamaraaalves.github.com.git
  ```

4. Navigate to the project folder:

  ```sh
  $ cd thamaraaalves.com
  ```

5. And finally run:

  ```sh
  $ jekyll
  ```

You'll have access to the website at `localhost:4000` :D

## Browser Support

![IE](https://raw.github.com/alrra/browser-logos/master/internet-explorer/internet-explorer_48x48.png) | ![Chrome](https://raw.github.com/alrra/browser-logos/master/chrome/chrome_48x48.png) | ![Firefox](https://raw.github.com/alrra/browser-logos/master/firefox/firefox_48x48.png) | ![Opera](https://raw.github.com/alrra/browser-logos/master/opera/opera_48x48.png) | ![Safari](https://raw.github.com/alrra/browser-logos/master/safari/safari_48x48.png)
--- | --- | --- | --- | --- |
IE 8+ ✔ | Latest ✔ | Latest ✔ | Latest ✔ | Latest ✔ |

## File structure

The basic file structure for the project is organized in the following way:

```
.
|-- _includes
|-- _layouts
|-- _plugins
|-- _posts
|-- _site
|-- assets
|-- _config.yml
`-- index.html
```

### [_includes](https://github.com/thamaraaalves/blog/tree/master/_includes)

They're blocks of code used to generate the main page of the site ([index.html](https://github.com/thamaraaalves/blog/blob/master/index.html)).

### [_plugins](https://github.com/thamaraaalves/blog/tree/master/_plugins)

Here you'll find all plugins used.

### [_posts](https://github.com/thamaraaalves/blog/tree/master/_posts)

Here you'll find a list of files for each post.

### [_layouts](https://github.com/thamaraaalves/blog/tree/master/_layouts)

Here you'll find the default template of the application.

### _site

Here you'll find all the static files generated by Jekyll after it's execution. However, this directory is unnecessary in our model, that's why it's ignored ([.gitignore](https://github.com/thamaraaalves/blog/blob/master/.gitignore)).

### [assets](https://github.com/thamaraaalves/blog/tree/master/assets)

Here you'll find all images, CSS and JS files.

### [_config.yml](https://github.com/thamaraaalves/blog/blob/master/_config.yml)

It stores most of the settings of the application.

### [index.html](https://github.com/thamaraaalves/blog/blob/master/index.html)

It's the file responsible for all application sections.

*More information about Jekyll's file structure [here](https://github.com/mojombo/jekyll/wiki/Usage).*

## Credits

Inspired by Andy Taylor, and Zeno Rocha.

## License

[MIT License](http://thamaraaalves.mit-license.org/) © Thamara Alves
