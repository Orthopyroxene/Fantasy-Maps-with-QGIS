# Project Overview: Interactive D&D-Styled Webmapping Application

## Objective
Develop an interactive webmapping service that allows users to explore fantasy maps styled in a D&D theme. Users can click on specific locations (e.g., buildings) to load detailed maps of these locations.

## Tools and Technologies
- **Inkarnate**: For creating fantasy maps.
- **QGIS**: To georeference the created maps using ground control points and integrate road and suburb data to structure map boundaries.
- **qgis2web**: To convert QGIS projects into web maps.
- **Web Development Environment**: HTML, CSS, JavaScript for embedding and enhancing the web maps with interactive features.

## Workflow
1. **Map Creation**: Design the initial fantasy maps using Inkarnate.
2. **Georeferencing**: Import the Inkarnate maps into QGIS and use ground control points for georeferencing.
3. **Data Integration**: Add road and suburb data to structure the map boundaries.
4. **Exporting Web Maps**: Use qgis2web to export the georeferenced maps into web-ready formats.
5. **Web Integration**: Embed the exported maps into the designated website.
6. **Interactivity Enhancement**: Implement JavaScript to add interactive features, allowing users to click on buildings to load new detailed maps.

## Expected Outcomes
- A fully interactive web-based map service that provides a user-friendly experience for exploring D&D-themed fantasy maps.
- Enhanced engagement through interactive elements, such as clickable locations that reveal detailed views.

## Processing Flowchart

```mermaid
graph TD;
    A[Create Map in Inkarnate] -->|Export as Image| B[Import to QGIS];
    B --> C[Add Road and Suburb Data];
    C --> D[Georeference using GCPs];
    D --> E[Export with qgis2web];
    E --> F[Embed in Website];
    F --> G[Add Interactive Features];
    G --> H[Interactive Web Map Ready];
