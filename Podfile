platform :ios, '10.0'
use_frameworks!

target 'the-blue-alliance-ios' do
  # pod 'TBAKit', :path => '/Users/zachorr/Desktop/TBAKit', :branch => 'swift'
  pod 'TBAKit', :git => 'https://github.com/ZachOrr/TBAKit.git', :branch => 'master'
  pod "youtube-ios-player-helper", "~> 0.1.4"
  pod 'PureLayout'
end

post_install do | installer |
  require 'fileutils'
  FileUtils.cp_r('Pods/Target Support Files/Pods-the-blue-alliance-ios/Pods-the-blue-alliance-ios-acknowledgements.plist',
  'the-blue-alliance-ios/Settings.bundle/Acknowledgements.plist', :remove_destination => true)
end
