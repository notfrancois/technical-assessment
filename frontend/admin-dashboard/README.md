# Frontend Admin Dashboard Exercise

## Overview

Build a responsive admin dashboard that displays and manages data with multiple views, filters, and visualizations. This exercise tests your abilities to create a complex interface with multiple interactive components working together cohesively.

## Technical Stack Requirements

-   **Framework**: React
-   **Build Tool**: Vite
-   **UI Library**: Material UI
-   **Data Source**: Mock data (no backend/API integration required)

## Requirements

### Core Features

-   **Navigation**: Implement a sidebar with at least 3 main sections (Dashboard, Analytics, Users)
-   **Dashboard View**:
    -   Summary cards showing key metrics (e.g., Total Users, Active Users, Revenue, etc.)
    -   At least one chart/graph visualization (line chart, bar chart, etc.)
    -   Recent activity feed or notification list
-   **Data Table**:
    -   Display tabular data with at least 5 columns
    -   Implement pagination (10 items per page)
    -   Allow sorting by at least 2 columns
    -   Include a search/filter functionality

### Data

You may use mock data for this exercise. Create a reasonable dataset with at least 50 records that includes:

-   User information (name, email, status, join date)
-   Activity metrics
-   Some numeric values that can be visualized in charts

## Technical Considerations

-   State management should be implemented efficiently
-   Use reusable components where appropriate
-   Loading states and error handling should be implemented
-   Implement at least one form with validation
-   You may use any chart library of your choice

## Mock Data

You are allowed to use mock data for this exercise. You can use the following interface to create the mock data:

```ts
interface User {
	id: number;
	name: string;
	email: string;
	status: string;
	joinDate: string;
}

interface Activity {
	id: number;
	userId: number;
	activity: string;
	date: string;
}

interface Metric {
	id: number;
	userId: number;
	metric: string;
	value: number;
}
```

## Plus Points (Not mandatory)

-   Dark/light theme toggle
-   Implement a settings panel
-   Add animations for transitions between views
-   Create an "edit user" modal
-   Implement data export functionality (CSV/JSON)
-   Add drag-and-drop functionality for dashboard widgets
