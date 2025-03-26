# Meteostations Status Dashboard

A simple static dashboard that displays information about meteostations from the provided JSON data.

## Features

- Table view of all stations with details including:
  - Station ID, name, and address
  - Geolocation with OpenStreetMap link
  - Installation date
  - Last signal timestamp
  - Active/Inactive status with color coding

- Interactive map (using Leaflet and OpenStreetMap) showing all station locations with:
  - Color-coded markers (green for active, red for inactive)
  - Clickable markers showing station details in a popup
  
- Statistics section displaying:
  - Count of active stations
  - Count of inactive stations
  - Total number of stations

## Deployment to GitHub Pages

Follow these steps to deploy this dashboard to GitHub Pages:

1. Create a GitHub repository for this project (if you haven't already)

2. Initialize Git in this directory (if not already initialized)
   ```bash
   git init
   ```

3. Add the files to the repository
   ```bash
   git add .
   ```

4. Commit the files
   ```bash
   git commit -m "Initial commit of meteostations dashboard"
   ```

5. Add your GitHub repository as a remote
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   ```

6. Push the files to GitHub
   ```bash
   git push -u origin main
   ```

7. Configure GitHub Pages:
   - Go to your repository on GitHub
   - Click on "Settings"
   - Scroll down to "Pages" section in the sidebar
   - Under "Source", select "Deploy from a branch"
   - Select the "main" branch and "/ (root)" folder
   - Click "Save"
   - Wait a few minutes for your site to be published
   - Your site will be available at https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/

## Notes

- The dashboard uses Leaflet with OpenStreetMap, which is completely free and doesn't require an API key.
- Make sure the meteostations.json file is included in your repository as it contains the data for the dashboard.
- The dashboard determines if a station is active based on whether its last signal was within the last 2 days.