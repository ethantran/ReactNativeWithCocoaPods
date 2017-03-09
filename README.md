# ReactNativeWithCocoaPods

https://github.com/facebook/react-native/issues/12814

Related links
https://stackoverflow.com/questions/42021796/react-native-xcode-project-product-archive-fails-with-duplicate-symbols-for-arch


Unable to archive with error ld: 397 duplicate symbols for architecture arm64

part of what error looks like
```
duplicate symbol _RCTReactTagAttributeName in:
    /Users/RONIN/Library/Developer/Xcode/DerivedData/ExampleWithCocoaPods-dpxtpuszieamoncxdckukxistgvr/Build/Intermediates/ArchiveIntermediates/ExampleWithCocoaPods/BuildProductsPath/Release-iphoneos/libReact.a(RCTShadowText.o)
    /Users/RONIN/Library/Developer/Xcode/DerivedData/ExampleWithCocoaPods-dpxtpuszieamoncxdckukxistgvr/Build/Intermediates/ArchiveIntermediates/ExampleWithCocoaPods/BuildProductsPath/Release-iphoneos/libRCTText.a(RCTShadowText.o)
```

Removing all libRCT*.a and libReact.a from 'Link Binary With Libraries' leads to error when building on both device and simulator

```
No component found for view with name "RCTRawText"
```

