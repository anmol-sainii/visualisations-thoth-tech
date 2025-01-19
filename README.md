# Student Task Progress Gauge Chart Prototype

This repository demonstrates a **prototype implementation of a gauge chart** to visualize student task progress. The gauge chart is intended to replace the current **pie chart** used on the dashboard. This prototype uses the **ngx-gauge** library and mock data to simulate its functionality.

## Purpose

The purpose of this project is to:
- Provide a more intuitive and compact visualization for student task progress.
- Replace the pie chart with a gauge chart, which highlights the progress value more effectively.
- Serve as a prototype for integrating the gauge chart into a production dashboard.

## Key Features

- **Gauge Chart**: Displays progress as a percentage in a circular format, focusing on a single value.
- **Improved Visualization**: Compared to the pie chart, the gauge chart provides a more direct and compact way to interpret progress.
- **Mock Data**: Simulates student task progress for testing and demonstration purposes.
- **Customizable**: Can be tailored to match the design and functionality of the final dashboard.

## Why Replace the Pie Chart?

- **Focus on a Single Metric**: The pie chart divides progress into segments, which can be less intuitive for users. The gauge chart emphasizes the progress percentage clearly.
- **Compact Design**: Gauge charts are space-efficient and visually appealing.
- **Improved Usability**: A gauge chart provides immediate feedback on progress without requiring detailed interpretation.

## Required Modules and Libraries

To integrate the gauge chart into an Angular application, the following modules and libraries are required:

1. **Angular Core Modules**:
   - Ensure your project is set up as an Angular application.

2. **ngx-gauge** Library:
   - Install the library using npm:
     ```bash
     npm install ngx-gauge
     ```

3. **App Module Configuration**:
   - Import the `NgxGaugeModule` in your `app.module.ts` file:
     ```typescript
     import { NgxGaugeModule } from 'ngx-gauge';

     @NgModule({
       declarations: [
         AppComponent,
       ],
       imports: [
         BrowserModule,
         NgxGaugeModule, // Import the Gauge Module
       ],
       providers: [],
       bootstrap: [AppComponent],
     })
     export class AppModule { }
     ```

4. **Dependencies**:
   - Ensure other Angular dependencies (like `@angular/core`, `@angular/common`, etc.) are installed and up-to-date.
## Running the Project on StackBlitz

StackBlitz is an online IDE that lets you run Angular projects directly in your browser without any setup. Follow the steps below to run this project on StackBlitz:

### Step 1: Create a New Angular Project
1. Visit [StackBlitz Angular Starter](https://stackblitz.com/fork/angular).
2. This will open a blank Angular project with basic files (`app.component.ts`, `app.component.html`, etc.).

### Step 2: Install `ngx-gauge`
1. Open the **Terminal** in StackBlitz (bottom right).
2. Run the following command to install the `ngx-gauge` library:
   ```bash
   npm install ngx-gauge
### Step 3: Set Up the Files

1. Copy the contents of the following files from this repository into your StackBlitz project:
   - **`app.component.ts`**: Paste into the existing `app.component.ts` file.
   - **`app.component.html`**: Paste into the existing `app.component.html` file.
   - **`data.ts`**: Create a new file named `data.ts` and paste the content.
   - **`app.module.ts`**: Update the existing `app.module.ts` to include the `NgxGaugeModule` as shown in the **Required Modules and Libraries** section.

### Step 4: Run the Application

1. Save all the changes in StackBlitz.
2. The app should automatically reload, and you will see the gauge chart displayed in the browser.

### Step 5: Test and Customize

- Modify the mock data in **`data.ts`** to test different progress values.

## Future Integration Steps

- Replace the **mock data** with real data from doubtfire API.
- Customize the gauge chart's **design, colors, and ranges** to align with the dashboard's theme.
- Test the chart's responsiveness across different devices and screen sizes.
- Integrate the chart into the main dashboard component where the pie chart is currently used.

## File Structure

- **`app.component.ts`**: Contains the logic for the gauge chart.
- **`app.component.html`**: Defines the template for the gauge chart.
- **`data.ts`**: Stores mock data simulating student task progress.
- **`app.module.ts`**: Configures the Angular app and imports necessary modules.


##Preview 
- Heres what it should look like
- <img width="830" alt="Screenshot 2025-01-19 at 10 22 23 PM" src="https://github.com/user-attachments/assets/89726960-9315-4838-a23a-8e5e2f99f220" />
