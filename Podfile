platform :ios, 10.0
use_frameworks!

target 'SwiftValidators' do
end

target 'SwiftValidatorsTests' do
    pod 'Quick', '~> 1.3.1'
    pod 'Nimble', '~> 7.3.0'
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '4.1'
        end
    end
end

