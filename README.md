# DC Bicycle & Micromobility Usage Dashboard

An interactive web dashboard for visualizing bicycle and micromobility usage patterns across Washington DC's road network. This dashboard combines observed counter data with predictive modeling to provide a comprehensive view of cycling activity throughout the city.

![Dashboard Preview](https://placeholder-image.com/dashboard-preview.jpg)

## Features

- **Interactive Map Visualization**: Color-coded bicycle volume predictions across the road network
- **Data Filtering**: Filter by neighborhood and counter type
- **Counter Point Display**: View locations of actual bicycle counting stations and their observed data
- **Detailed Segment Analysis**: Click on any street segment to view detailed metrics
- **Temporal Analysis**: View predicted bicycle counts by day of week and hour of day
- **Comparative Statistics**: Compare segment metrics with city-wide averages

## Getting Started

### Prerequisites

- Web browser with JavaScript enabled
- No server-side dependencies required (static HTML/CSS/JS application)

### Installation

1. Clone the repository or download the files
   ```
   git clone https://github.com/yourusername/dc-bike-dashboard.git
   ```

2. Open `index.html` in your web browser
   ```
   cd dc-bike-dashboard
   open index.html
   ```

### Directory Structure

```
dc-bike-dashboard/
├── index.html            # Main HTML file
├── style.css             # Main CSS styles
├── js/                   # JavaScript files
│   ├── main.js           # Main application logic
│   ├── map.js            # Map initialization and interaction
│   ├── data.js           # Data loading and processing
│   └── map-visualization.js  # Map visualization enhancements
├── data/                 # Data files
│   ├── road_network.geojson     # Road network data
│   ├── counter_points.geojson   # Bicycle counter locations
│   ├── neighborhoods.geojson    # Neighborhood boundaries
│   └── time_predictions.csv     # Temporal predictions data
└── images/               # Image assets including logo
    └── weitzman-logo.svg # Weitzman School of Design logo
```

## Usage

### Map Navigation

- **Pan**: Click and drag on the map
- **Zoom**: Use the zoom controls or mouse wheel to zoom in/out
- **Select Segment**: Click on any road segment to view detailed information
- **View Counter Data**: Click on counter points (circles) to see observed counts

### Data Filtering

- Use the **Neighborhood** dropdown to focus on specific areas
- Use the **Counter Type** dropdown to filter between automatic and manual counters

### Detailed Analysis

- **Segment Details**: Click on any road segment to view detailed statistics
- **Temporal Analysis**: In the segment details panel, switch to the "Temporal" tab to view time-based predictions
- **Counter Information**: View actual count data where available

### Mobile Usage

The dashboard is optimized for mobile devices:
- Responsive design adapts to different screen sizes
- Touch-friendly controls for map navigation
- Simplified interface on smaller screens

## Data Sources

- Bicycle counter data from DDOT (District Department of Transportation)
- Road network data from DC GIS
- Census demographics from US Census
- Predicted bicycle volumes from usage modeling

## Development

### Technologies Used

- **Leaflet.js**: Map visualization library
- **D3.js**: Data visualization components
- **PapaParse**: CSV parsing
- **HTML5/CSS3/JavaScript**: Core web technologies

### Customization

To customize the dashboard:

1. **Change Map Style**: Modify the tile layer URL in `map.js`
2. **Adjust Color Scheme**: Update the color functions in `map.js`
3. **Add New Data Layers**: Extend the data loading functions in `data.js`

## Contributing

Contributions to improve the dashboard are welcome. Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Team

This dashboard was developed by the Practicum Team:
- Hao Zhu
- Kuma Luo
- Shuya Guan
- Xian Lu Lee

For the Weitzman School of Design, University of Pennsylvania.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- District Department of Transportation (DDOT) for providing bicycle count data
- DC GIS for road network and boundary data
- Leaflet.js and OpenStreetMap contributors
