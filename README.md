# Synchronizing Blazor Grid and Charts

This repository demonstrates how to build an interactive data dashboard by synchronizing a [Blazor Grid](https://www.syncfusion.com/blazor-components/blazor-datagrid) with a [Charts](https://www.syncfusion.com/blazor-components/blazor-charts) component. Select any continent in the grid to dynamically view its corresponding population data visualization in real-time.

## Overview

Modern data applications require seamless interaction between multiple components. This sample showcases how to create a synchronized grid-and-chart interface where:

- **Grid Selection** triggers chart updates
- **Real-time synchronization** between components
- **Formatted data** with billion/million abbreviations for readability
- **World population data** organized by continents and countries

## Features

-  **Synchronized Components** - Grid selection instantly updates the chart
-  **Column Chart Visualization** - Displays country populations with data labels
-  **Real-world Dataset** - World population data by continent
-  **Smart Formatting** - Automatic conversion to B/M/K notation for large numbers
-  **Interactive UI** - Hover tooltips and responsive design
-  **Tailwind Theme** - Modern styling with Tailwind CSS 3

## Prerequisites

- [.NET SDK 8.0](https://dotnet.microsoft.com/download/dotnet/8.0) or later
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or later
- [Visual Studio Code](https://code.visualstudio.com/)

## Getting started

### Clone the repository

```bash
git clone https://github.com/SyncfusionExamples/Synchronizing-Blazor-Grid-And-Charts-Selecting-A-Row-To-Update-The-Chart.git
cd Synchronizing-Blazor-Grid-And-Charts-Selecting-A-Row-To-Update-The-Chart
```

### Run with Visual Studio

1. Open the solution file using Visual Studio 2022 or later.
2. Restore the NuGet packages by rebuilding the solution.
3. Build the project to ensure there are no compilation errors.
4. Run the project.

### Run with .NET CLI

```bash
# Restore dependencies
dotnet restore

# Run the project
dotnet run
```

## References

- Blazor Synchronized chart Documentation: https://blazor.syncfusion.com/documentation/chart/how-to/synchronized-chart
- Blazor DataGrid Documentation: https://blazor.syncfusion.com/documentation/datagrid/getting-started
- Blazor Chart Data Binding: https://blazor.syncfusion.com/documentation/chart/working-with-data
