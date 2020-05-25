# ios-papers-on-big4
Notes for papers from big-4 conferences (S&P, CCS, USENIX, NDSS) that are related to iOS

# iRis: Vetting private API Abuse in iOS Applications, CCS 2015
* 静态检测+动态插桩。利用动态插桩monitor the registration of UI event Handler，制作UI event handler exploration approach。
* Porting Valgrind to iOS, the first intruction-level dynamic binary instrumentation framework on iOS.

## iOS Class hierarchy
MyClass my_instance

my_instance.isa -> MyClass_MetaClass

MyClass_MetaClass.super -> FatherClass

## iOS Dynamic Libs
Dylib exposes APIs in two ways:
1. as traditional C APIs, which are exported explicitly
2. as OC methods, which are dispatched at runtime

