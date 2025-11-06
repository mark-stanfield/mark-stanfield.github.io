# Gemfile
source "https://rubygems.org"

# Use Jekyll
gem "jekyll", "~> 4.3" # Use the latest 4.x version

# Explicitly include common plugins used with GitHub Pages
# This avoids potential conflicts within the github-pages meta-gem
group :jekyll_plugins do
  gem 'jekyll-feed', '~> 0.12'
  gem 'jekyll-sitemap', '~> 1.4'
  gem 'jekyll-seo-tag', '~> 2.7'
  gem 'jekyll-remote-theme', '~> 0.4' # Useful if you use remote themes
  # gem 'jekyll-paginate', '~> 1.1' # If you need pagination
  # gem 'jekyll-archives', '~> 2.2' # If you need post archives
end

# Optional: You *can* still try including github-pages,
# but often it's better to list plugins explicitly as above.
# If you remove the explicit plugins above, you could try just:
# gem "github-pages", group: :jekyll_plugins
# However, the explicit list is generally more reliable for avoiding conflicts like this.

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :install_if => Gem.win_platform?
