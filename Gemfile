source "https://rubygems.org"

if ENV['FOG_LIBVIRT_DEPS_GIT'] == '1'
  gem "fog-core", :github => "fog/fog-core"
  gem "fog-json", :github => "fog/fog-json"
else
  gem "fog-core", "~> 1.27", ">= 1.27.4"
  gem "fog-json"
end

group :development, :test do
  # This is here because gemspec doesn't support require: false
  gem "coveralls", :require => false
  gem "netrc", :require => false
  gem "octokit", :require => false
end

gemspec
