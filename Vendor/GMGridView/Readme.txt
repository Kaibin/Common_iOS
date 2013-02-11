
iOSGridView,github,http://www.apps168.net/post/1111.html
GMGridView
How to integrate GMGridView in project

1 copy GMGridView folder from https://github.com/gmoledina/GMGridView to your project dir
2 in xcode right click on any file group and choose add files
3 find GMGridView folder in your folder dir and choose GMGridView.xcodeproj - (dont copy, create groups not folders, add targets)
4 go to your project targets - search - HEADER_SEARCH_PATHS add-  GMGridView/**
5 select Building phases in settings - choose target dependencies and add GMGridView
6 select Building phases in settings - link binary libraries and add libGMGridView.a
7 TARGETS->Bulid Settings->Other Linker Flags, then add -ObjC -all_load

https://github.com/gmoledina/GMGridView/issues/54
http://stackoverflow.com/questions/10990332/how-to-link-third-party-libraries-properly-in-ios/11016498#11016498