source "https://rubygems.org"

# Use github-pages gem for compatibility with GitHub Pages build env.
# Specifying this gem lets Dependabot alert you when versions change.
gem "github-pages", group: :jekyll_plugins

# Optional plugins compatible with GitHub Pages
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-seo-tag"
end

# Windows-specific gems (ignored on Linux CI)
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]
