source "http://rubygems.org"


gem "rake"
gem "git", ">= 1.2.5"
gem "bundler", "~> 1.0"
gem "rdoc"

group :development do
  gem "yard", "~> 0.7.4"
  gem "rdoc"
  gem "bluecloth"
  gem "cucumber", "~> 1.1.4"
  gem "rcov"
end

group :test do
  gem "timecop"
  gem "activesupport", "~> 2.3.5"
  gem "shoulda"
  gem "mhennemeyer-output_catcher"
  gem "rr", "~> 1.0.4"
  gem "mocha"
  gem "redgreen"
  gem "test-construct"
  gem "rake"
end

# yo dawg, i herd u lieked jeweler
group :xzibit do
  # steal a page from bundler's gemspec:
  # add this directory as jeweler, in order to bundle exec jeweler and use the current working directory
  gem 'jeweler', :path => '.'
end


group :debug do
  platforms :mri_18 do
    gem "ruby-debug"
  end
  platforms :mri_19 do
    gem "ruby-debug19"
    gem (RUBY_VERSION == "1.9.2" ? "ruby-debug-base19" : "ruby-debug-base19x")
  end
end
