source "http://rubygems.org"

#bundle config mirror.https://rubygems.org https://gems.ruby-china.com  #换成中国源，不然贼慢（终端运行）

# Hello! This is where you manage which Jekyll version is used to run.
# When you want to use a different version, change it below, save the
# file and run `bundle install`. Run Jekyll with `bundle exec`, like so:
#
#     bundle exec jekyll serve
#
# This will help ensure the proper Jekyll version is running.
# Happy Jekylling!

# gem "jekyll"
gem "jekyll-katex"
gem "rack"
gem "webrick"
# If you want to use GitHub Pages, remove the "gem "jekyll"" above and
# uncomment the line below. To upgrade, run `bundle update github-pages`.
gem "github-pages", group: :jekyll_plugins
# If you have any plugins, put them here!
group :jekyll_plugins do
  gem "jekyll-feed"
  gem 'jekyll-admin', "0.9.0"
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", :install_if => Gem.win_platform?



# source "http://rubygems.org"
# # 你好！这是管理使用哪个 Jekyll 版本运行的地方。
# # 当你想使用不同的版本时，在下面更改它，保存文件并运行 `bundle install`。
# # 使用 `bundle exec` 运行 Jekyll，如下所示：
# #
# #     bundle exec jekyll serve
# #
# # 这将有助于确保运行正确的 Jekyll 版本。
# # Jekyll 使用愉快！

# gem "jekyll"
# gem "rack"
# gem "webrick"
# # 如果你想使用 GitHub Pages，请删除上面的 "gem "jekyll"" 并
# # 取消下面这行的注释。要升级，请运行 `bundle update github-pages`。
# # gem "github-pages", group: :jekyll_plugins
# # 如果你有任何插件，请放在这里！
# group :jekyll_plugins do
#   gem "jekyll-feed"
#   gem 'jekyll-admin', "0.9.0"
# end

# # Windows 和 JRuby 不包含 zoneinfo 文件，因此捆绑 tzinfo-data gem
# # 和相关库。
# install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
#   gem "tzinfo", "~> 1.2"
#   gem "tzinfo-data"
# end

# # 提高在 Windows 上监视目录的性能
# gem "wdm", :install_if => Gem.win_platform?
