# ReactNativeWithCocoaPods

https://github.com/facebook/react-native/issues/12814

Unable to archive with error ld: 397 duplicate symbols for architecture arm64

part of what error looks like
```
duplicate symbol _RCTReactTagAttributeName in:
    /Users/RONIN/Library/Developer/Xcode/DerivedData/ExampleWithCocoaPods-dpxtpuszieamoncxdckukxistgvr/Build/Intermediates/ArchiveIntermediates/ExampleWithCocoaPods/BuildProductsPath/Release-iphoneos/libReact.a(RCTShadowText.o)
    /Users/RONIN/Library/Developer/Xcode/DerivedData/ExampleWithCocoaPods-dpxtpuszieamoncxdckukxistgvr/Build/Intermediates/ArchiveIntermediates/ExampleWithCocoaPods/BuildProductsPath/Release-iphoneos/libRCTText.a(RCTShadowText.o)
```