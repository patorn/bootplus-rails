# Bootplus::Rails

Bootplus for Rails Asset Pipeline extracted from [bootplus](https://github.com/aozora/bootplus)

## Installation

Add this line to your application's Gemfile:

    gem 'bootplus-rails'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install bootplus-rails

## Usage

Create bootplus_overrides.less with the following codes

    @import "bootstrap";
    @import "bootplus/bootplus";
    @import "bootplus/responsive";

    // Set the correct sprite paths
    @iconSpritePath: "glyphicons-halflings.png";
    @iconWhiteSpritePath: "glyphicons-halflings-white.png";

    // Set the Font Awesome (Font Awesome is default. You can disable by commenting below lines)
    // Note: If you use asset_path() here, your compiled bootstrap_and_overrides.css will not
    //       have the proper paths. So for now we use the absolute path.
    @fontAwesomeEotPath: "fontawesome-webfont.eot?v=3.0.2";
    @fontAwesomeEotPath_iefix: "fontawesome-webfont.eot?#iefix&v=3.0.2";
    @fontAwesomeWoffPath: "fontawesome-webfont.woff?v=3.0.2";
    @fontAwesomeTtfPath: "fontawesome-webfont.ttf?v=3.0.2";

Add bootplus_overrides.less to your `application.css`

    *= require bootplus_overrides

Add bootstrap.js to your `application.js`
    
    //= require bootstrap

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## ROADMAP

1. Add generator
