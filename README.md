# Graviton Analytics Dashboard – MS FinCap

A comprehensive financial analytics dashboard for MS FinCap, built with React and Tailwind CSS. This dashboard provides real-time insights into business performance, collections, credit risk, and operations.

## 🚀 Features

### Dashboard Views
- **CXO Overview** - Executive-level metrics including AUM, disbursements, WIRR, PAR, and collection efficiency
- **Business Performance** - Comprehensive analysis with dynamic filters and multiple views:
  - Comparative Analytics (Nov vs Oct trends)
  - Approval Analysis with donut charts
  - Conversion Funnel visualization
  - RO Productivity tracking
  - TAT (Turnaround Time) Analysis
- **Collections** - Collection efficiency, bucket-wise portfolio, and resolution rates
- **Credit & Risk** - Bureau score analysis, deviation tracking, and credit TAT
- **Operations** - NACH penetration, FTR rates, and operational exceptions

### Key Capabilities

#### 🎛️ Dynamic Filtering
- Filter by State, Branch, Date Range, and Comparison Period
- Real-time data updates across all charts
- Slider control for flexible date range selection (7-90 days)

#### 📊 Interactive Charts
- **Bar Charts** - Comparative analysis with visible values
- **Line Charts** - Trend analysis over time
- **Donut Charts** - Approval breakdown and distribution
- **Funnel Charts** - Visual conversion tracking
- All charts display values directly (no hover required)

#### 🌓 Dark Mode Support
- Complete dark mode implementation
- Persistent theme preference (localStorage)
- Smooth transitions between themes
- Charts adapt to theme with proper colors

#### 📈 Business Analytics
- **Comparative Period Analysis** - Automatic comparison logic
- **Approval Metrics** - Donut chart showing Approved/Rejected/WIP
- **Conversion Funnel** - Login → Sanction → Disbursement flow
- **RO Productivity** - Login and disbursement range distribution
- **TAT Analysis** - Stage-wise turnaround time tracking

#### 📋 Data Tables
- Sortable and filterable data tables
- Color-coded performance indicators
- Progress bars for visual metrics
- Hover effects for better UX

## 🛠️ Technology Stack

- **React 18** - UI library
- **Tailwind CSS** - Utility-first CSS framework
- **Chart.js** - Data visualization
- **Babel Standalone** - JSX transformation

## 📦 Getting Started

### Installation

No build process required! This is a standalone HTML file.

1. Clone the repository:
```bash
git clone https://github.com/Migration-Graviton/Mock_Graviton_Dashboard.git
cd Mock_Graviton_Dashboard
```

2. Open `index.html` in your web browser:
```bash
# On Windows
start index.html

# On macOS
open index.html

# On Linux
xdg-open index.html
```

Or simply drag and drop `index.html` into your browser.

### Development

The application is a single-page application (SPA) built entirely in one HTML file. No build tools or package managers needed.

To make changes:
1. Open `index.html` in your favorite code editor
2. Modify the React components in the `<script type="text/babel">` section
3. Refresh your browser to see changes

## 📊 Data Structure

The dashboard uses real data from the tabular format:

```javascript
{
  state: "GJ",
  branch: "Direct",
  loginCount_Nov: 69,
  loginAmount_Nov: 8.71,
  loginCount_Oct: 69,
  sanctionCount: 15,
  sanctionAmount: 0.66,
  totalDisb: 0.42,
  wirr_Nov: 20.58,
  wip_Count: 21,
  // ... more fields
}
```

## 🎨 UI Components

### Reusable Components
- **Card** - Container for dashboard sections
- **KPI** - Key performance indicator with tooltip
- **LineChart** - Time series visualization
- **BarChart** - Comparative bar charts
- **DonutChart** - Circular distribution charts

### Dashboard Sections
- **CxoDashboard** - Management overview
- **BusinessDashboard** - Multi-view business analytics
- **CollectionsDashboard** - Collection metrics
- **CreditDashboard** - Credit risk analysis
- **OpsDashboard** - Operational metrics

## 🌟 Key Features Detail

### Business Performance Dashboard

#### 1. Comparative Analytics
- Side-by-side comparison of current vs previous period
- Percentage change indicators with visual arrows
- State-wise performance breakdown
- Login, Sanction, and Disbursement trends

#### 2. Approval Analysis
- Donut chart visualization
- Breakdown: Approved / Rejected / WIP
- State-wise approval rates
- Progress bar indicators

#### 3. Conversion Funnel
- Visual funnel representation
- Login → Sanction → Disbursement flow
- Conversion percentages at each stage
- State-wise conversion rates

#### 4. RO Productivity
- Login range distribution (0-10, 11-20, 21-30, etc.)
- Disbursement amount ranges
- Individual RO performance table
- Productivity ratings (High/Medium/Low)

#### 5. TAT Analysis
- Login → Sanction TAT
- Login → Decision TAT
- Sanction → Disbursement TAT
- SOP Compliance tracking
- Target vs Actual comparison

## 🎯 Filter Options

All charts support dynamic filtering:
- **State** - Filter by geographic region
- **Branch** - Filter by specific branch
- **Date Range** - Slider for 7-90 days
- **Comparison Period** - Previous Period / Same Period Last Year

## 🎨 Design Features

- Modern gradient designs
- Responsive grid layouts
- Color-coded status indicators
- Smooth hover effects
- Professional typography
- Accessible color contrast

## 📱 Responsive Design

The dashboard is fully responsive and works on:
- Desktop (1920px+)
- Laptop (1366px - 1920px)
- Tablet (768px - 1366px)
- Mobile (320px - 768px)

## 🔄 Updates & Maintenance

To update data:
1. Locate the `rawData` array in the `BusinessDashboard` component
2. Update values with new data
3. Save and refresh

To add new states/branches:
1. Add entries to the `rawData` array
2. Filters will automatically update

## 📝 License

MIT License - feel free to use this dashboard for your projects.

## 👥 Contributors

Built for MS FinCap by the Graviton Analytics team.

## 🐛 Known Issues

None currently. Please report issues via GitHub Issues.

## 🚀 Future Enhancements

- [ ] Export to PDF functionality
- [ ] Data export to Excel
- [ ] More granular date filters
- [ ] Product-wise analysis
- [ ] Category-wise breakdown
- [ ] Advanced search functionality
- [ ] User role-based views

## 📞 Support

For support or questions, please open an issue on GitHub.

---

**Last Updated:** November 16, 2025  
**Version:** 1.0.0
