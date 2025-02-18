
# Flight Scheduler UI

This is a web application for scheduling and managing flight reservations. The UI provides:

- A calendar-based time slot scheduler showing available flight slots
- Support for both student and instructor views
- Ability to view and manage flight reservations across multiple days
- Interactive tooltips showing reservation details on hover
- URL configuration options for different hosting environments

The interface allows users to:

- Browse available time slots in a calendar view
- Make flight reservations by selecting time slots
- View existing reservations and their details
- Navigate between different dates using forward/back controls
- Configure the backend API endpoint via URL parameters

The application is built using React and includes real-time updates of reservation data through periodic API calls to the backend server.

# Getting Started

Follow these steps to run the application locally on your machine.

## Running the Akka app locally or on the platform

Clone the companion project [akka-dev-cert](https://github.com/akka/akka-dev-cert.git).

Follow the steps provided in that repo's README for developing and running the certification service.

When your Akka service is up and running, follow the steps below to run the UI.

## Running the UI

1. **Prerequisites**
   - Make sure you have [Node.js](https://nodejs.org/) installed (version 14 or higher)
   - A terminal/command prompt application

2. **Clone the Repository**

   ```bash
   git clone https://github.com/akka/akka-dev-cert-ui.git
   cd akka-dev-cert-ui
   ```

3. **Install Dependencies**

   ```bash
   npm install
   ```

   This may take a few minutes to complete.

4. **Start the Development Server**

   ```bash
   npm run dev
   ```

5. **Access the Application Locally**
   - Open your web browser
   - Navigate to `http://localhost:3000`
   - You should now see the application running

6. **Access the Application running on the Akka platform
   - Create an externally accessible hostname using the `akka services expose` command
   - Use the `akka services get akka-dev-cert` command to get the hostname of your service
   - Open your web browser
   - Navigate to `http://localhost:3000?host=[hostname]`
   - You should now see the application running

The development server will automatically reload if you make any changes to the source files.

To stop the application, go to the terminal and press `Ctrl + C` (or `Cmd + C` on Mac).

## Troubleshooting

If you encounter any issues:

1. Make sure all prerequisites are installed correctly
2. Try deleting the `node_modules` folder and `package-lock.json` file, then run `npm install` again
3. Ensure no other applications are running on port 3000
4. Check the terminal for error messages

## Caveat Emptor

This repository and its code are provided as-is and are not covered by Akka security policies. There are no guarantees of security, stability, or support. Use at your own risk.
