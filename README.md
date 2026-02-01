# Cloud Provider Map

## Overview

**Cloud Provider Map** is an interactive visualization tool that displays datacenter locations from major cloud providers across the globe. This tool helps developers, architects, and IT professionals explore and compare the geographic distribution of cloud infrastructure from providers including AWS, Azure, Google Cloud Platform, IBM Cloud, Oracle Cloud, and Alibaba Cloud.

## Purpose

The primary goals of this tool are to:

- **Visualize Global Infrastructure**: See at a glance where major cloud providers have established their datacenters
- **Compare Provider Coverage**: Understand which providers have presence in specific regions or countries
- **Explore Location Types**: Learn about different infrastructure types (Regions, Edge Locations, Local Zones, Availability Zones)
- **Support Decision Making**: Help inform cloud provider selection based on geographic requirements
- **Educational Resource**: Provide clear definitions of how each provider categorizes their infrastructure

## Features

### Interactive Map
- **Global View**: Pan and zoom across a world map showing all datacenter locations
- **Color-Coded Markers**: Each cloud provider has a distinct color for easy identification
- **Pin-Style Icons**: Custom markers with provider-specific colors and location-type icons
- **Click for Details**: Select any marker to view detailed information about that location

### Advanced Filtering
- **Provider Selection**: Toggle individual cloud providers on/off
- **Location Type Filtering**: Filter by infrastructure type (Region, Edge Location, etc.)
- **Independent Controls**: Each provider's location types can be filtered independently
- **Persistent Filters**: Your filter preferences are saved between sessions

### Information Panel
- **Location Details**: View name, provider, type, location, and available services
- **Provider Definitions**: See how each provider defines their infrastructure types
- **Overview Statistics**: When no location is selected, view aggregate statistics including:
  - Total visible locations
  - Breakdown by provider
  - Breakdown by location type
  - Geographic distribution

### Reset Functionality
- **Quick Reset**: Two reset buttons allow you to instantly restore all filters and clear selections
- **Fresh Start**: Return to the default view showing all providers and location types

## How to Use

### Getting Started

1. **Open the Website**: Navigate to the Cloud Provider Map in your web browser
2. **Explore the Map**: The map loads with all providers and location types visible by default
3. **Pan and Zoom**: Use your mouse or touch gestures to navigate the map

### Filtering Locations

#### By Provider
1. Locate the **Filters** panel on the left side
2. Under **Providers & Locations**, you'll see each cloud provider listed
3. Click the checkbox next to a provider name to show/hide all their locations
4. Click the arrow icon to expand/collapse the provider's location types

#### By Location Type
1. Expand a provider by clicking anywhere on their header row
2. You'll see location types available for that provider (Region, Edge Location, etc.)
3. Check/uncheck individual location types to filter what appears on the map
4. Each provider's location types are controlled independently

#### Understanding Location Types

- **Region**: Primary datacenter locations with full service availability
- **Edge Location**: Content delivery and caching locations for low-latency access
- **Local Zone**: Extensions of regions for ultra-low latency applications
- **Availability Zone**: Isolated locations within a region for high availability

*Note: Hover over the info icon (ⓘ) next to each location type to see provider-specific definitions*

### Viewing Location Details

1. **Click a Marker**: Click any pin on the map to select that location
2. **View Information**: The **Provider Information** panel at the bottom displays:
   - Location name and geographic details
   - Provider and infrastructure type
   - Provider-specific definition of the location type
   - Link to view available services (when applicable)
3. **Clear Selection**: Click the reset icon next to "Provider Information" or select another marker

### Viewing Overview Statistics

1. **Deselect All Markers**: Click a reset icon or click outside all markers
2. **View Summary**: The information panel shows:
   - Total number of visible locations
   - Count of locations per provider
   - Count of locations per type
   - Top countries by location count

### Resetting Filters

- **Reset Icon (Filters)**: Click the circular arrow next to "Filters" to reset all selections
- **Reset Icon (Provider Information)**: Click the circular arrow next to "Provider Information" to reset and show overview
- **Reset All Filters Button**: Click the gray button at the bottom of the filter panel

All reset actions will:
- Enable all cloud providers
- Enable all location types for each provider
- Clear any selected location
- Show the overview statistics

## Cloud Providers Included

| Provider | Identifier | Color |
|----------|-----------|-------|
| Amazon Web Services (AWS) | `aws` | Orange |
| Microsoft Azure | `azure` | Blue |
| Google Cloud Platform (GCP) | `gcp` | Green |
| IBM Cloud | `ibm-cloud` | Black |
| Oracle Cloud | `oracle-cloud` | Red |
| Alibaba Cloud | `alibaba-cloud` | Orange |

## Data Sources

All datacenter location information is sourced from publicly available documentation provided by the respective cloud providers. This includes:

- Official provider documentation
- Public cloud infrastructure maps
- Service availability matrices
- Regional endpoint listings

**Note**: Datacenter locations, availability, and services may change. Always verify critical information with official provider documentation.

## Browser Compatibility

Cloud Provider Map works best on modern web browsers:

- **Chrome/Edge**: Version 90+
- **Firefox**: Version 88+
- **Safari**: Version 14+
- **Mobile Browsers**: iOS Safari 14+, Chrome Mobile 90+

## Feedback & Contributions

### Submit Feedback

We welcome your feedback, suggestions, and bug reports! Here's how you can contribute:

#### Via GitHub Issues

1. **Visit Our Repository**: Navigate to `https://github.com/[YOUR-USERNAME]/[YOUR-REPO-NAME]/issues`
2. **Check Existing Issues**: Search to see if your feedback has already been reported
3. **Create New Issue**: Click the "New Issue" button
4. **Choose Issue Type**:
   - **Bug Report**: For errors or unexpected behavior
   - **Feature Request**: For new functionality suggestions
   - **Documentation**: For improvements to documentation or help content
   - **Data Update**: For outdated or incorrect datacenter information

#### Issue Template Guidelines

**For Bug Reports**, please include:
- Description of the issue
- Steps to reproduce
- Expected behavior vs. actual behavior
- Browser and version
- Screenshots (if applicable)

**For Feature Requests**, please include:
- Clear description of the proposed feature
- Use case or problem it solves
- Any relevant examples or mockups

**For Data Updates**, please include:
- Provider name
- Location name or identifier
- What needs to be updated (coordinates, name, type, etc.)
- Link to official provider documentation

#### Via Email

You can also send feedback directly to: `feedback@example.com`

### Contributing Code

If you'd like to contribute code improvements:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request with a clear description

## Disclaimer

This tool is provided for informational purposes only. While we strive to maintain accurate and up-to-date information:

- Datacenter locations and services may change without notice
- This tool is not affiliated with or endorsed by any cloud provider
- Always verify critical information with official provider documentation
- No warranty is provided for the accuracy or completeness of the data

For the complete disclaimer, click the "Disclaimer" link in the footer.

## Support

- **Website Issues**: Submit via GitHub Issues (see above)
- **General Questions**: Contact via email at `feedback@example.com`
- **Connect**: Find us on [LinkedIn](https://www.linkedin.com/in/lawther/)

## Credits

Built with:
- [Leaflet](https://leafletjs.com/) - Interactive map library
- [OpenStreetMap](https://www.openstreetmap.org/) - Map tiles and data
- [Kiro](https://kiro.dev) - AI-powered development assistant

---

**Last Updated**: February 2026

**Version**: 1.0.0

---

*Explore. Compare. Decide. Find the right cloud infrastructure for your needs.*
