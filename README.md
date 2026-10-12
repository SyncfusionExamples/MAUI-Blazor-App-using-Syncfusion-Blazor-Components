# MAUI Blazor App Using Syncfusion Blazor Components

## Overview

This sample demonstrates how Syncfusion [Blazor components](https://www.syncfusion.com/blazor-components) can be integrated into a .NET MAUI Blazor hybrid application. The repository contains multiple MAUI Blazor examples that showcase Syncfusion UI controls running inside a native MAUI application while using Blazor for the user interface layer.

The primary scenario illustrates how Syncfusion components can be rendered and configured within a cross-platform MAUI Blazor project, enabling developers to build desktop and mobile applications using a shared Blazor-based UI. The sample serves as a reference for combining native MAUI hosting capabilities with Syncfusion Blazor controls.

## Key Features

- Demonstrates the Syncfusion Blazor Calendar component using the `SfCalendar<TValue>` control with `TValue="DateTime"` for date selection.
- Shows how to render the Syncfusion Blazor Calendar component within a .NET MAUI Blazor hybrid application.
- Demonstrates the Syncfusion Blazor Chart component using the `SfChart` control with a chart title configured through the `Title` property.
- Configures a categorical X-axis using `ChartPrimaryXAxis` with `ValueType="Category"` and a custom axis title.
- Configures a numeric Y-axis using `ChartPrimaryYAxis` with a custom title for displaying sales values.
- Uses a column chart visualization through the `ChartSeries` component with `Type="ChartSeriesType.Column"`.
- Binds chart data using the `DataSource` property and maps data fields through the `XName` and `YName` properties.
- Demonstrates strongly typed chart data using the `SalesInfo` model containing `Month` and `SalesValue` properties.
- Displays monthly sales data using an in-memory `List<SalesInfo>` collection.
- Demonstrates the Syncfusion Blazor DataGrid component using the `SfGrid` control.
- Binds the DataGrid through the `DataSource` property using a strongly typed `List<Order>` collection.
- Generates sample Grid records dynamically in the `OnInitialized()` lifecycle method.
- Demonstrates data modeling using the `Order` class with `OrderID`, `CustomerID`, `OrderDate`, and `Freight` properties.
- Populates sample order data using LINQ's `Enumerable.Range()` method.
- Shows integration of multiple Syncfusion Blazor components within .NET MAUI Blazor Hybrid applications using shared Razor component architecture.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/) 
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download the repository.
2. Open the project located under the appropriate sample folder:
   - `GridExample/MauiBlazorApp`
   - `Calendar Example`
   - `Chart Example`
3. Open the corresponding `.csproj` file if a solution file is not available.
4. Restore NuGet packages.
5. Build the project.
6. Select the desired MAUI target platform.
7. Press `Ctrl+F5` to build and run the application.

**Visual Studio Code**

1. Clone the repository.
2. Open the repository folder in Visual Studio Code.
3. Navigate to the desired project directory.

```bash
cd GridExample/MauiBlazorApp
dotnet restore
dotnet run
```

4. Open the URL displayed in the terminal after the application starts.

## Project Structure

`Calendar Example/MauiCalendarApp/Pages/Index.razor` - Hosts the Syncfusion `SfCalendar<DateTime>` component for date selection.

`Chart Example/MauiChartApp/Pages/Index.razor` - Hosts the Syncfusion `SfChart` component that visualizes monthly sales data using a column series.

`Chart Example/MauiChartApp/Pages/Index.razor` - Defines the `SalesInfo` data model with `Month` and `SalesValue` properties used by the chart.

`Chart Example/MauiChartApp/Pages/Index.razor` - Creates and populates an in-memory `List<SalesInfo>` data source for chart binding.

`GridExample/MauiBlazorApp/Pages/Home.razor` - Hosts the Syncfusion `SfGrid` component and binds order data through the `DataSource` property.

`GridExample/MauiBlazorApp/Pages/Home.razor` - Implements the `OnInitialized()` lifecycle method to generate sample Grid records.

`GridExample/MauiBlazorApp/Pages/Home.razor` - Defines the `Order` model containing `OrderID`, `CustomerID`, `OrderDate`, and `Freight` fields.

`GridExample/MauiBlazorApp/Pages/Home.razor` - Generates sample order data using `Enumerable.Range()` and assigns the collection to the Grid data source.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- [Getting Started with .NET MAUI Blazor App](https://blazor.syncfusion.com/documentation/getting-started/maui-blazor-app)

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.