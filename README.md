### Project Summary: Attendance Location Tracking App

The Attendance Location Tracking App is a Flutter-based application designed to monitor and visualize the locations and routes traveled by individual members. Users can access the app from a menu and click on the Attendance option, which displays a list of members, each accompanied by two icons. The second icon allows users to check the current location and travel history of a selected member.

Upon selecting a member, the app presents a map showing their current location, along with a timeline view of all visited locations, defaulting to today's data. Users can utilize a date filter to explore past travel data, and they can pull the list to view a comprehensive history of traveled locations.

The app also enables users to select any two visited locations to generate a route, displayed on a separate screen. This screen details the start and stop locations, total kilometers traveled, and total duration. Additionally, the route is visually represented on the map, with red dots indicating stop times for periods exceeding ten minutes. This functionality provides a comprehensive solution for tracking attendance and travel behavior, enhancing accountability and transparency.



attendance_app/
├── android/                     # Android-specific files
├── ios/                         # iOS-specific files
├── lib/
│   ├── models/                  # Data models
│   │   ├── member.dart          # Member model
│   │   └── location.dart        # Location model
│   ├── screens/                 # UI screens
│   │   ├── attendance_screen.dart # Attendance listing screen
│   │   ├── location_screen.dart  # Member location screen
│   │   ├── route_details_screen.dart # Route details screen
│   │   └── home_screen.dart      # Home screen (menu)
│   ├── services/                # Services for data fetching and business logic
│   │   ├── location_service.dart # Service for fetching locations
│   │   └── member_service.dart   # Service for member-related data
│   ├── utils/                   # Utility classes/functions
│   │   ├── constants.dart        # Constants used throughout the app
│   │   ├── date_formatter.dart    # Date formatting utility
│   │   └── api_client.dart       # API client for HTTP requests
│   ├── widgets/                 # Reusable widgets
│   │   ├── member_tile.dart      # Widget for displaying a member
│   │   ├── location_marker.dart   # Widget for location markers
│   │   └── timeline_view.dart     # Widget for timeline view
│   ├── main.dart                 # Main entry point of the app
│   └── app.dart                  # App configuration and theme
├── pubspec.yaml                  # Project dependencies
└── README.md                     # Project documentation
