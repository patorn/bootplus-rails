# Bootplus::Rails

Bootplus for Rails Asset Pipeline extracted from [bootplus](https://github.com/aozora/bootplus)
Use this gem [less-rails-fontawesome](https://github.com/wbzyl/less-rails-fontawesome) for font awesome

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'therubyracer'
gem 'less-rails'
gem 'less-rails-fontawesome'
gem 'bootplus-rails'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install bootplus-rails

## Usage

Create bootplus_overrides.less with the following codes

```css
@import 'bootplus/bootplus';
@import 'bootplus/responsive';
@import 'font-awesome/font-awesome';
@import 'font-awesome/font-awesome-ie7';

// Set the correct sprite paths
@iconSpritePath: "glyphicons-halflings.png";
@iconWhiteSpritePath: "glyphicons-halflings-white.png";
```
Add bootplus_overrides.less to your `application.css`

```css
*= require bootplus_overrides
```

Add bootstrap.js to your `application.js`
    
```js
//= require bootplus/bootstrap
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## ROADMAP

1. Add generator
