source "https://rubygems.org"

# GitHub Pages
gem "github-pages", group: :jekyll_plugins

# Use local theme for development, remote theme for production
if ENV["JEKYLL_ENV"] == "production"
  # For production (GitHub Pages)
  gem "just-the-docs", git: "https://github.com/nwoodfine/style-the-docs.git", branch: "master"
else
  # For local development - adjust the path to where your theme is located
  gem "just-the-docs", path: "../style-the-docs"
end

# Required for Ruby 3.0+
gem "webrick"

# Add REXML dependency for Ruby 3.x
gem "rexml"

# Add jekyll-include-cache (required by newer Just the Docs)
gem "jekyll-include-cache" 