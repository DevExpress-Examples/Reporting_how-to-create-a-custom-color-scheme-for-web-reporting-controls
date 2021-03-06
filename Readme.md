<!-- default file list -->
*Files to look at*:
* [_Layout.cshtml](./CS/WebReportingCustomColorScheme/Views/Shared/_Layout.cshtml)
* [Viewer.cshtml](./CS/WebReportingCustomColorScheme/Views/Home/Viewer.cshtml)
* [Designer.cshtml](./CS/WebReportingCustomColorScheme/Views/Home/Designer.cshtml)
* [devextreme.light.custom.css](/CS/WebReportingCustomColorScheme/Content/devextreme.light.custom.css)
* [reporting.light.custom.css](/CS/WebReportingCustomColorScheme/Content/reporting.light.custom.css)
<!-- default file list end -->

# How to Create a Custom Color Scheme for Web Report Designer and Document Viewer

This example demonstrates how to create a custom color scheme for the [Web Document Viewer](https://docs.devexpress.com/XtraReports/17738) and [End-User Report Designer](https://docs.devexpress.com/XtraReports/17103). The custom color scheme is based on the "_light_" predefined color scheme.

This example is an **ASP.NET MVC application**. However, the approach used to customize the color scheme is the same for all Web platforms.

![](/images/screenshot.png)

The **Color Scheme Customization** online demo is used to customize a color scheme and save the result. Online demos are available for different platforms:

* [ASP.NET WebForms Online Demo](https://demos.devexpress.com/xtrareportsdemos/WebSpecificFeatures/ColorSchemeCustomization.aspx)
* [ASP.NET MVC Online Demo](https://demos.devexpress.com/MVCxReportDemos/WebSpecificFeatures/ColorSchemeCustomization)
* [ASP.NET Core Online Demo](https://demos.devexpress.com/ASPNetCore/Demo/Reporting/ColorSchemeCustomization)

The demo produces custom styles in two files - _devextreme.light.custom.css_ and _reporting.light.custom.css_. Copy these files to the application's **Content** folder.

* The **devextreme.light.custom.css** file contains changed CSS styles for <a href="https://js.devexpress.com/">DevExtreme</a> UI widgets that reporting controls internally use.

* The **reporting.light.custom.css** file contains changed CSS styles (grouped by categories) that define the common appearance of reporting controls.

Specify the base color scheme with the [GetStyleSheets](https://docs.devexpress.com/AspNet/DevExpress.Web.Mvc.UI.ExtensionsFactory.GetStyleSheets.overloads) method and link the reporting and DevExtreme CSS files to the Document Viewer and Report Designer pages.

**See also:**

* [ASP.NET Webforms Documentation](https://docs.devexpress.com/XtraReports/116672)
* [ASP.NET MVC Documentation](https://docs.devexpress.com/XtraReports/400235)
* [ASP.NET Core Documentation](https://docs.devexpress.com/XtraReports/400413)

