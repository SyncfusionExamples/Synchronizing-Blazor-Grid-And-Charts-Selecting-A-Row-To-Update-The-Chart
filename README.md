# Synchronizing Blazor Grid and Charts

This repository demonstrates how to build an interactive data dashboard by synchronizing a Blazor Grid with a Chart component. Select any continent in the grid to dynamically view its corresponding population data visualization in real-time.

## Overview

Modern data applications require seamless interaction between multiple components. This sample showcases how to create a synchronized grid-and-chart interface where:

- **Grid Selection** triggers chart updates
- **Real-time synchronization** between components
- **Formatted data** with billion/million abbreviations for readability
- **World population data** organized by continents and countries

## Features

-  **Synchronized Components** - Grid selection instantly updates the chart
-  **Column Chart Visualization** - Displays country populations with data labels
-  **Real-world Dataset** - World population data by continent (2025 estimates)
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

## How it works

The application implements a simple yet effective pattern for component synchronization:

1. **Grid Component** displays continents with their total population
2. **User clicks a grid row** triggering the `RowSelectHandler` event
3. **Event handler updates** the chart data source based on selected continent
4. **Chart re-renders** showing the top 5 countries for that continent
5. **Data formatting** displays values in B/M/K notation for better readability

### Key Components

- `Home.razor` - Main page containing both Grid and Chart components
- `ChartData` class - Model for chart data (Country, Population)
- `ContinentData` class - Model for grid data (Continent, Total Population)
- `PopulationData` dictionary - Maps continents to their countries' data

## References

- [Blazor Event Handling](https://learn.microsoft.com/en-us/aspnet/core/blazor/components/event-handling)
- [Blazor Data Binding](https://learn.microsoft.com/en-us/aspnet/core/blazor/components/data-binding)