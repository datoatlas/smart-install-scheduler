# Smart Install Scheduler

Route optimization and scheduling tool for installation teams in Ireland using Eircodes.

## Features

- **Team Management**: Add multiple installation teams with depot locations
- **Job Entry**: Add jobs with Eircode, duration, and optional time windows
- **Route Optimization**: Greedy nearest-neighbor algorithm for efficient routing
- **Geocoding**: Automatic Eircode to coordinate conversion using OpenStreetMap
- **Schedule Generation**: Calculate start/end times with travel time estimates
- **CSV Export**: Download complete schedules for sharing with teams

## How It Works

1. Add your installation teams and their depot Eircodes
2. Add jobs with location (Eircode), duration, and team assignment
3. Set working hours and date
4. Click "Optimize Routes" to generate optimal schedules
5. Export to CSV for distribution

## Technical Details

- **Geocoding**: Nominatim (OpenStreetMap) API
- **Distance Calculation**: Haversine formula for accurate distance
- **Route Optimization**: Greedy nearest-neighbor algorithm
- **Travel Time**: Estimated at 50 km/h average speed
- **No API keys required**: Completely free to use

## Limitations

- Uses straight-line distance calculations (not actual road routes)
- Travel time is estimated, not based on real-time traffic
- Rate limited to 1 geocoding request per second
- Basic optimization (not globally optimal, but fast and practical)

## Use Cases

- Installation companies scheduling daily routes
- Service teams planning maintenance visits
- Delivery route optimization
- Field service management

## Tech Stack

Pure HTML/CSS/JavaScript - no dependencies, frameworks, or build tools required.

## License

All rights reserved
