# Doctor Dashboard

## Overview

Doctor Dashboard is a web application designed to manage medical facilities, schedules, and appointments. It provides a comprehensive interface for doctors, administrators, and patients to interact and manage their medical-related activities efficiently.

## Features

- **Dashboard**: Overview of the system with quick access to various functionalities.
- **Manage Schedules**: Allows doctors to manage their schedules.
- **Manage Medical Facilities**: Administrators can manage medical facilities and assign doctors to them.
- **Authentication**: Supports Google authentication for secure login.
- **Real-time Notifications**: Uses SignalR for real-time updates and notifications.
- **Responsive Design**: Optimized for various devices and screen sizes.

## Technologies Used

- **ASP.NET Core Razor Pages**: For building the web application.
- **Entity Framework Core**: For database operations.
- **SignalR**: For real-time web functionality.
- **AutoMapper**: For object-object mapping.
- **Bootstrap**: For responsive design.
- **jQuery**: For client-side scripting.
- **Chart.js**: For data visualization.
- **Google Authentication**: For secure login.

## Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

### Installation

1. Clone the repository:
    git clone https://github.com/yourusername/doctor-dashboard.git
cd doctor-dashboard
2. Set up the database:
    - Update the connection string in `appsettings.json`:  "ConnectionStrings": {
    "DefaultConnection": "Server=your_server;Database=your_database;User Id=your_user;Password=your_password;"
  }
     - Apply migrations:  dotnet ef database update3. Configure Google Authentication:
    - Update the `appsettings.json` with your Google Client ID and Secret:
        "Authentication": {
    "Google": {
      "ClientId": "your_client_id",
      "ClientSecret": "your_client_secret"
    }
  }
4. Run the application: dotnet run
5. Open your browser and navigate to `https://localhost:5001`.

## Project Structure

- **Application**: Contains the main application code including Razor Pages, models, and services.
- **BusinessLogic**: Contains business logic and services.
- **DataAccessObject**: Contains data access layer including repositories and database context.
- **wwwroot**: Contains static files like CSS, JavaScript, and images.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries or issues, please contact [your-email@example.com](mailto:your-email@example.com).

