# -*- coding: utf-8 -*-
$:.unshift("/Library/RubyMotion/lib")
require 'motion/project/template/ios'

begin
  require 'bundler'
  Bundler.require
rescue LoadError
end

Motion::Project::App.setup do |app|
  # Use `rake config' to see complete project settings.
  app.name = 'zbar'

  app.frameworks += [
    "AVFoundation",
    "CoreMedia",
    "CoreVideo",
    "QuartzCore",
  ]

  app.libs << "/usr/lib/libiconv.dylib"

  app.pods do
    pod "ZBarSDK"
  end
end
