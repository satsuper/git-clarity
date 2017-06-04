# Technical Choices

The supported operating systems will be Windows only for the foreseeable future as I use it as my primary operating system so I am not motivated to provide support for other platforms.

I wish to create this tool using C# so I did a brief evaluation of the following UI frameworks:

* GtkSharp
    * Looks and feels best on GNOME.
* Mono/XWT
    * Poor documentation.
* WinForms
    * Stable but frustrating to deal with layouts, high DPI scenarios.
* Xamarin.Forms
    * Unstable desktop environment support.
 * UWP(Universal Windows Platform)
    * Limited APIs due to security model.
* WPF
    * A dead end platform but full featured and usable.
* Eto.Forms
    * This is super impressive but unsure I want an cross-platform abstraction that I won't use.
* Avalonia
    * Looks cool but in the alpha stages.

There are other worthy tool kits like Qt but not really ready for consumption from C#.

From my brief investigation it feels like the current state of .NET UI tool kits is not great. The best options are WinForms and WPF but both are dead end technologies in the new cross platform .NET world. UWP is great for Windows Store applications but nothing else.

Xamarin.Forms has a timeline with desktop support but I believe that is at least a year away from being usable.

The choice for now will be WPF with a goal to structure the application in a way to allow alternative UIs or different frameworks in the future.

The supported platforms will be MS supported desktop Windows operating systems which is currently Windows 7 and onwards.
