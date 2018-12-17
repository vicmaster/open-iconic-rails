# Open Iconic Rails

##### Open Iconic is the open source sibling of [Iconic](http://useiconic.com). It is a hyper-legible collection of 223 icons with a tiny footprint&mdash;ready to use with Bootstrap and Foundation. [View the collection](http://useiconic.com/open#icons)

##### Open Iconic Rails provides a view helper for placing SVG icons within your template files.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'open-iconic-rails'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install open-iconic-rails

## Config

Asset id not declared to be precompiled until you do:

Add `Rails.application.config.assets.precompile += %w( open-iconic.min.svg )` to `config/initializers/assets.rb` and restart your server

## Usage

##### open_iconic :svg_class, :icon_name

open_iconic :icon, :account_login

or

open_iconic "icon", "account-login"

```
  <svg class="icon" viewBox="0 0 8 8">
    <use class="icon-account-login" xlink:href="/assets/open-iconic.min.svg#account-login">
    </use>
  </svg>
```
## Todo

1. Add sample code for bootstrap & foundation
2. Explore adding aria tags for accessibility
3. Possibly add support for the other icon formats (icon font, img sprites)

## Contributing

1. Fork it ( https://github.com/[my-github-username]/open-iconic-rails/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
