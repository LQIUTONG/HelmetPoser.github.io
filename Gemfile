source "https://rubygems.org" # source "https://gems.ruby-china.com"

gemspec

gem "github-pages", group: :jekyll_plugins

# 添加兼容性补丁 for Ruby 3.2
if Gem::Version.new(RUBY_VERSION) >= Gem::Version.new('3.0.0')
  gem "webrick", "~> 1.7"
  gem "faraday-retry"
  
  # 在Ruby 3.2中处理tainted?方法缺失的问题
  if RUBY_VERSION >= "3.2.0"
    gem "liquid", "~> 4.0.4"
    gem "jekyll", "~> 4.3"
  end
end
