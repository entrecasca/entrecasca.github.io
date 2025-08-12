source "https://rubygems.org"

# Use GitHub Pages gem which includes Jekyll and other dependencies
gem "github-pages", group: :jekyll_plugins

# Required for Jekyll 4.x compatibility
gem "webrick", "~> 1.8"

# Additional plugins
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-sitemap"
  gem "jekyll-include-cache"
  gem "jekyll-paginate"
  gem "jekyll-remote-theme"
end

# Windows and JRuby support
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]