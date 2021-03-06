# jekyll-gutenberg

[Gutenberg][] is a meaningful web typography starter kit. This project packages Gutenberg as a Jekyll theme.

To accommodate customizations, add a `_sass/_gutenberg-customizations.scss` file (`.sass` works too). See [docs][] to learn more about what can be configured.

If you would like to override this theme's `style.scss` with your own stylesheet, add this line to invoke Gutenberg:

```scss
@import "gutenberg-jekyll";
```

## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-gutenberg"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-gutenberg
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jekyll-gutenberg

## Usage

TODO: Write usage instructions here. Describe your available layouts, includes, sass and/or assets.

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/mfilej/jekyll-gutenberg. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## Development

To set up your environment to develop this theme, run `bundle install`.

To update Gutenberg source files, run `rake update`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.
To add a custom directory to your theme-gem, please edit the regexp in `jekyll-gutenberg.gemspec` accordingly.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

[Gutenberg]: https://matejlatin.github.io/Gutenberg/
[docs]: https://github.com/matejlatin/Gutenberg/wiki#base-sizes
