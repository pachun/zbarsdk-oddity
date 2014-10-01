zbarsdk-oddity
==============

git clone git@github.com:pachun/zbarsdk-oddity.git

cd zbarsdk-oddity

bundle

rake pod:install

rake

(Yay!! builds just fine!)

quit (to close simulator)

rake clean:all

[delete you app's /vendor directory just to explicitly take as back to a state file/dir wise that I understand to be **exactly** the same as before we built anything]

bundle (I don't think we need this agian, but just to be sure -- looks exactly the same to me as the process earlier)

rake pod:install

rake

(wtf.)

```
     Build ./build/iPhoneSimulator-8.0-Development
2014-10-01 12:59:58.442 xcodebuild[96165:1007] [MT] PluginLoading: Required plug-in compatibility UUID C4A681B0-4A26-480E-93EC-1218098B9AA0 for plug-in at path '~/Library/Application Support/Developer/Shared/Xcode/Plug-ins/XVim.xcplugin' not present in DVTPlugInCompatibilityUUIDs
     Build ./vendor/Pods/Pods.xcodeproj [ZBarSDK - Release]
2014-10-01 12:59:58.715 xcodebuild[96165:30b] error: InputFile    /Users/pachun/Desktop/zbarsdk-oddity/vendor/Pods/Target Support Files/Pods-ZBarSDK/Pods-ZBarSDK-prefix.pch 0 1412182592 382 33188... malformed line 10; 'InputFile' should have exactly five arguments
2014-10-01 12:59:58.716 xcodebuild[96165:30b] error: InputFile    /Users/pachun/Desktop/zbarsdk-oddity/vendor/Pods/Target Support Files/Pods-ZBarSDK/Pods-ZBarSDK-prefix.pch 0 1412182592 382 33188... malformed line 10; 'InputFile' should have exactly five arguments
   Compile ./vendor/Pods/Target Support Files/Pods-ZBarSDK/Pods-ZBarSDK-dummy.m
   Compile ./vendor/Pods/ZBarSDK/iphone/ZBarCVImage.m
   Compile ./vendor/Pods/ZBarSDK/iphone/ZBarCameraSimulator.m
   Compile ./vendor/Pods/ZBarSDK/iphone/ZBarHelpController.m
   Compile ./vendor/Pods/ZBarSDK/iphone/ZBarImage.m
   Compile ./vendor/Pods/ZBarSDK/iphone/ZBarReaderView.m
   Compile ./vendor/Pods/ZBarSDK/iphone/ZBarImageScanner.m
   Compile ./vendor/Pods/ZBarSDK/iphone/ZBarReaderController.m
** BUILD FAILED **


The following build commands failed:
        CompileC build/Pods.build/Release-iphonesimulator/Pods-ZBarSDK.build/Objects-normal/i386/Pods-ZBarSDK-dummy.o Target\ Support\ Files/Pods-ZBarSDK/Pods-ZBarSDK-dummy.m normal i386 objective-c com.apple.compilers.llvm.clang.1_0.compiler
        CompileC build/Pods.build/Release-iphonesimulator/Pods-ZBarSDK.build/Objects-normal/i386/ZBarCVImage.o ZBarSDK/iphone/ZBarCVImage.m normal i386 objective-c com.apple.compilers.llvm.clang.1_0.compiler
        CompileC build/Pods.build/Release-iphonesimulator/Pods-ZBarSDK.build/Objects-normal/i386/ZBarCameraSimulator.o ZBarSDK/iphone/ZBarCameraSimulator.m normal i386 objective-c com.apple.compilers.llvm.clang.1_0.compiler
        CompileC build/Pods.build/Release-iphonesimulator/Pods-ZBarSDK.build/Objects-normal/i386/ZBarHelpController.o ZBarSDK/iphone/ZBarHelpController.m normal i386 objective-c com.apple.compilers.llvm.clang.1_0.compiler
        CompileC build/Pods.build/Release-iphonesimulator/Pods-ZBarSDK.build/Objects-normal/i386/ZBarImage.o ZBarSDK/iphone/ZBarImage.m normal i386 objective-c com.apple.compilers.llvm.clang.1_0.compiler
        CompileC build/Pods.build/Release-iphonesimulator/Pods-ZBarSDK.build/Objects-normal/i386/ZBarReaderView.o ZBarSDK/iphone/ZBarReaderView.m normal i386 objective-c com.apple.compilers.llvm.clang.1_0.compiler
        CompileC build/Pods.build/Release-iphonesimulator/Pods-ZBarSDK.build/Objects-normal/i386/ZBarImageScanner.o ZBarSDK/iphone/ZBarImageScanner.m normal i386 objective-c com.apple.compilers.llvm.clang.1_0.compiler
        CompileC build/Pods.build/Release-iphonesimulator/Pods-ZBarSDK.build/Objects-normal/i386/ZBarReaderController.o ZBarSDK/iphone/ZBarReaderController.m normal i386 objective-c com.apple.compilers.llvm.clang.1_0.compiler
(8 failures)
    ERROR! Building vendor project `vendor/Pods' failed to create at least one `.a' library.
```
