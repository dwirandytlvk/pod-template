${HEADER_PODS}

def module_dependency_pod
  pod 'MUIKit', :path => '../MUIKit'
  pod 'TVLFoundation', :path => '../TVLFoundation'
  pod 'TVLNetwork', :path => '../TVLNetwork'
  pod 'TVLStorage', :path => '../TVLStorage'
  pod 'TVLUI', :path => '../TVLUI'
  pod 'TVLKit', :path => '../TVLKit'
  pod 'YogaKit', :path => '../YogaKit'

  # SwiftLinting
  pod 'SwiftLint', "= 0.37.0"

  # Yoga
  pod 'Yoga', :path => '../../react-native/ReactCommon/yoga', :modular_headers => false

  # Add third party pods here
  # pod 'AFNetworking', '= 3.2.1'
end

target 'SandboxApp' do
  module_dependency_pod

  pod '${POD_NAME}', :path => '.'

  ${INCLUDED_PODS}
end

target '${POD_NAME}' do
  module_dependency_pod

  target '${POD_NAME}Tests' do
    pod 'Nimble', '= 8.0.1'
    pod 'OCMock', '= 3.4.1'
    pod 'Quick', '= 2.2.0'
  end
end
