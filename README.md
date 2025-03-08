# ucWebView2
tB WebView2 Control Wrapper OCX

Wayne Phillips created a wonderful WebView2 control for twinBASIC, but it uses tB's new WindowsControl framework, which isn't compiled to an ocx that can be used by other apps. This project creates an ActiveX control wrapper around the tB control, so it can be compiled into an OCX that can be used in VB6 and VBA (both 32 and 64 bit): Designed to be an open source alternative to the RC6 implementation for VB6/VBA32, with added support for VBA64.

![image](https://github.com/user-attachments/assets/9a79a7da-2359-4612-88ce-5f627ed5072b)

![image](https://github.com/user-attachments/assets/7068b124-74df-4aec-87c1-2869c049a596)

## BETA ##

The currently posted version is for **BETA TESTING** and may have bugs and is lacking features.

This control is built around my WebView2WDL package, which is just the original control package set to use WinDevLib instead of built in definitions, since WinDevLib already has more recent versions of the WebView2 interfaces built in. 

WebView2WDLPackage.twinproj - Source for WDL version of WebView2 control package.

WebView2WDLPackage.twinpack - WebView2 twinBASIC control for use inside tB.

WebView2SamplesWDL.twinproj - twinBASIC IDE `Sample #1a: WebView2 Samples`, with WebView2WDLPackage replacing the native tB package.

**WebView2Control.twinproj** - The wrapper UserControl/ActiveX control project file hosting an instance of WebView2WDLPackage. This has its own copy; you don't need any of the other files unless you want to edit the control source.


