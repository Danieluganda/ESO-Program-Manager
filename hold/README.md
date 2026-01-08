# ESO Program Management App

A modern, responsive web application for managing Enterprise Support Organization (ESO) program activities, events, and outreach.

## Features

### 📊 Dashboard
- Quick overview of all activities, events, and ESO outreach
- Real-time statistics
- Recent activities and upcoming events at a glance

### 📅 Schedule Management
- View all Schedule C activities with codes, tasks, and deliverables
- Filter by priority (High, Medium, Low)
- Search functionality
- Track progress and deadlines

### 🎯 Events Calendar
- Visual card-based event display
- Filter by workstream (Incubation, Communications, Learning)
- Detailed event information including objectives, audience, and logistics
- Search functionality

### 🤝 ESO Outreach
- Track all ESO partnership activities
- Monitor status (Completed, Ongoing, Pending)
- Contact information and lead assignments
- Location-based filtering

### 📈 Reports & Analytics
- Program completion rates
- Priority breakdowns
- Timeline visualization
- Active partner statistics

## How to Use

### Opening the App

1. **Open `index.html` in any modern web browser**
   - Double-click the file, or
   - Right-click and select "Open with" → Your browser
   - Recommended browsers: Chrome, Firefox, Safari, Edge

### Navigation

- **Sidebar Menu**: Click on any menu item to navigate between pages
  - Dashboard: Overview and statistics
  - Schedule: All scheduled activities
  - Events: Event calendar
  - ESO Outreach: Partner outreach activities
  - Reports: Analytics and visualizations

- **Mobile**: Click the menu icon (☰) in the header to open/close the sidebar

### Searching and Filtering

- Use the **search bar** on each page to find specific items
- Use **dropdown filters** to narrow down results:
  - Schedule: Filter by priority
  - Events: Filter by workstream
  - ESO: Filter by status

### Viewing Details

- Click on any **activity card** or **table row** to view full details in a popup modal
- Click the "View" button in tables for detailed information
- Close modals by clicking the × or clicking outside the modal

### Data Actions

- **Add New**: Click the "+ Add" buttons to add new items (demo mode)
- **Edit**: Click "Edit" buttons to modify existing items (demo mode)
- **Download Excel**: Click the download button in the sidebar to export data

## Files Included

```
📁 ESO Program Manager/
├── index.html         # Main HTML structure
├── styles.css         # All styling and design
├── app.js            # JavaScript functionality and data
└── README.md         # This file
```

## Data Structure

The app uses data extracted from your three Excel files:

1. **Incubators_and_Accelerators_Schedule_C_activities.xlsx**
   - 37 schedule activities with codes, tasks, and priorities

2. **Events_Tracker.xlsx**
   - 15 events across different workstreams

3. **ESO_tasks_Calendar__1_.xlsx**
   - 82 ESO outreach activities with contact information

## Customization

### Adding More Data

To add more data to the app, edit the `appData` object in `app.js`:

```javascript
const appData = {
    schedule: [ /* your schedule items */ ],
    events: [ /* your events */ ],
    eso: [ /* your ESO activities */ ]
};
```

### Changing Colors

Edit the CSS variables in `styles.css`:

```css
:root {
    --primary-color: #4472C4;  /* Main brand color */
    --success-color: #28a745;  /* Success indicators */
    --warning-color: #ffc107;  /* Warning indicators */
    --danger-color: #dc3545;   /* High priority items */
}
```

## Browser Compatibility

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## Responsive Design

The app is fully responsive and works on:
- 💻 Desktop computers
- 💻 Laptops
- 📱 Tablets
- 📱 Mobile phones

## Future Enhancements

To make this a fully functional app with real data management:

1. **Backend Integration**: Connect to a server/database
2. **Real-time Updates**: Auto-refresh data
3. **Export to Excel**: Download updated spreadsheets
4. **User Authentication**: Login system for multiple users
5. **Notifications**: Email/SMS alerts for deadlines
6. **Calendar Integration**: Sync with Google Calendar/Outlook
7. **File Upload**: Import new Excel files directly
8. **Data Visualization**: Charts and graphs for analytics

## Support

For questions or issues:
- Review the organized Excel workbook: `ESO_Program_Management_Organized.xlsx`
- Check that all three files (HTML, CSS, JS) are in the same folder
- Ensure JavaScript is enabled in your browser

## License

This app is created for internal use in the ESO Program Management.

---

**Version**: 1.0  
**Last Updated**: November 2024  
**Created for**: ESO Program Team
