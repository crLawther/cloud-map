# Version History

## Unreleased Changes (Since Last Commit: 56095fe)

### Date: February 3, 2026

### Features Added

#### 1. Marker Clustering Implementation
- **Added Leaflet MarkerCluster Plugin** to handle overlapping datacenter locations
- Markers within 35 pixels now cluster together with numbered badges
- Automatic "spiderfy" behavior fans out overlapping markers when zoomed in
- Cluster icons use provider-specific colors for easy identification
- Smooth transitions between clustered and individual marker states

**Files Modified:**
- `index.html` - Added MarkerCluster CSS and JavaScript libraries
- `js/map-manager.js` - Replaced LayerGroup with MarkerClusterGroup
- `css/styles.css` - Added custom cluster styling

**Configuration:**
- `maxClusterRadius: 35` - Markers within 35 pixels cluster together
- `spiderfyOnMaxZoom: true` - Overlapping markers fan out at maximum zoom
- `spiderfyDistanceMultiplier: 1.5` - Controls fan-out spacing
- `zoomToBoundsOnClick: true` - Clicking cluster zooms to show all markers

**Benefits:**
- Resolves issue with overlapping markers in same geographic area (e.g., Washington DC region)
- Improves map readability at all zoom levels
- Maintains ability to select individual locations when zoomed in
- Preserves provider-specific color coding in cluster badges

### Bug Fixes

#### 1. GitHub Actions Workflow Branch Configuration
- **Fixed branch name** from `main` to `master` to match repository default branch
- **Fixed file path case** from `disclaimer.md` to `DISCLAIMER.md` for consistency

**Files Modified:**
- `.github/workflows/sync-docs.yml`

**Changes:**
```yaml
# Before
branches: [main]
paths: ['disclaimer.md']

# After  
branches: [master]
paths: ['DISCLAIMER.md']
```

---

## Previous Changes (Included in Commit 56095fe)

See git history for details on:
- Initial marker clustering CSS setup
- Footer link updates
- Data model standardization
- UI improvements
- Filter behavior changes

---

## How to Use This Document

This changelog tracks all modifications made to the Cloud Provider Map application. Each entry includes:
- **Feature/Fix Description** - What was changed and why
- **Files Modified** - Which files were updated
- **Configuration Details** - Specific settings and values
- **Benefits** - Impact on user experience

When committing changes, move items from "Unreleased Changes" to a new version section with the commit hash.
