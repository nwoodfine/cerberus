source "https://rubygems.org"

# Match the Jekyll version that GitHub Pages uses. The github-pages gem is not
# used here because it pins jekyll-remote-theme 0.4.3, which needs a vulnerable
# rubyzip (< 3.0).
gem "jekyll", "~> 3.10"
gem "kramdown-parser-gfm"

# Plugins that GitHub Pages enables, plus the ones this site needs
group :jekyll_plugins do
  gem "jekyll-remote-theme", "~> 0.6"
  gem "jekyll-include-cache"
  gem "jekyll-github-metadata"
  gem "jekyll-optional-front-matter"
  gem "jekyll-readme-index"
  gem "jekyll-default-layout"
  gem "jekyll-titles-from-headings"
  gem "jekyll-relative-links"
  gem "jekyll-seo-tag"
end

# Use git theme for both development and production
gem "just-the-docs", git: "https://github.com/nwoodfine/style-the-docs.git", branch: "master"

# Required for Ruby 3.0+
gem "webrick"

# Add REXML dependency for Ruby 3.x
gem "rexml"

# Security fix: CVE-2026-85396 (path traversal) is fixed in rubyzip 3.4.0
gem "rubyzip", ">= 3.4.0"
