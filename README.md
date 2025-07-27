# Boostify - Advanced SEO Audit Tool

Boostify is a comprehensive SEO audit tool that provides detailed analysis, competitor comparison, analytics dashboard, and advanced export capabilities.

## Features

### 🔍 Core SEO Audit
- **Keyword Analysis**: Extract and analyze relevant keywords
- **Meta Tags**: Check title tags, meta descriptions, and H1 tags
- **Content Quality**: Word count, readability analysis
- **Technical SEO**: Mobile-friendliness, structured data, canonical tags
- **Link Analysis**: Internal and external link counting
- **Image Optimization**: Alt text analysis and image count

### 📊 Advanced Visualizations
- **Interactive Charts**: Radar charts, bar charts, pie charts, line charts
- **Real-time Analytics**: Trend analysis and performance tracking
- **Customizable Dashboards**: Multiple chart types and export options
- **Responsive Design**: Optimized for all device sizes

### 🏆 Competitor Analysis
- **Multi-site Comparison**: Compare your site against competitors
- **Performance Metrics**: SEO, content quality, and technical scores
- **Ranking Analysis**: Position tracking and improvement suggestions
- **AI-Powered Recommendations**: Smart suggestions based on competitor data

### 📈 Analytics Dashboard
- **Historical Trends**: Track performance over time
- **SQLite Database**: Persistent storage of audit results
- **Date Range Filtering**: 7d, 30d, 90d, 1y analysis periods
- **Summary Statistics**: Average, max, min scores and total audits

### 📤 Enhanced Export & Reporting
- **Multiple Formats**: PDF, PowerPoint (PPTX), HTML, JSON
- **Report Templates**: Default, Executive, and Detailed templates
- **Scheduled Reports**: Daily, weekly, monthly automated reports
- **Professional Layouts**: Branded reports with charts and recommendations
- **Email Integration**: Optional email delivery for scheduled reports

### 🎨 Modern UI/UX
- **Dark Mode**: Toggle with persistence across sessions
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Accessibility**: ARIA roles, keyboard navigation, screen reader support
- **Smooth Animations**: Hover effects and transitions
- **Professional Branding**: Clean, modern interface

## Installation

1. **Clone the repository**:
```bash
git clone <repository-url>
cd Boostify
```

2. **Install dependencies**:
```bash
pip install -r requirements.txt
```

3. **Set up environment variables**:
Create a `.env` file in the root directory:
```
DEEPSEEK_API_KEY=your_deepseek_api_key_here
```

4. **Run the application**:
```bash
python main.py
```

5. **Access the application**:
Open your browser and navigate to `http://localhost:8000`

## Usage

### Basic SEO Audit
1. Enter a URL in the main interface
2. Click "Run SEO Audit"
3. View results in the interactive dashboard
4. Export results in your preferred format

### Competitor Analysis
1. Enter your target URL
2. Add competitor URLs (up to 5)
3. Click "Compare with Competitors"
4. Review comparison metrics and recommendations

### Analytics Dashboard
1. Navigate to the Analytics tab
2. Select a date range for analysis
3. View trend charts and historical data
4. Export analytics reports

### Enhanced Export Options
1. **Quick Export**: Use the export buttons for immediate downloads
2. **Template Reports**: Choose from Default, Executive, or Detailed templates
3. **Scheduled Reports**: Set up automated reports with custom frequency
4. **Multiple Formats**: Export as PDF, PowerPoint, HTML, or JSON

## API Endpoints

### Core Audit
- `POST /seo-audit` - Run SEO audit on a URL
- `POST /full-scan` - Full website crawl and audit
- `GET /scan-status/{job_id}` - Check scan progress

### Competitor Analysis
- `POST /competitor-analysis` - Start competitor comparison
- `GET /competitor-status/{job_id}` - Check competitor analysis status

### Analytics
- `POST /analytics/trends` - Get analytics trends
- `GET /analytics/history/{url}` - Get audit history for a URL

### Enhanced Export
- `POST /export/report` - Generate reports in various formats
- `POST /export/schedule` - Schedule automated reports
- `GET /export/scheduled/{report_id}` - Retrieve scheduled reports
- `GET /export/templates` - Get available report templates
- `DELETE /export/schedule/{report_id}` - Cancel scheduled reports

## Report Templates

### Default Report
- Complete SEO analysis with all metrics
- Available formats: PDF, PowerPoint, HTML, JSON
- Best for: Comprehensive analysis and technical teams

### Executive Summary
- High-level performance overview
- Available formats: PDF, PowerPoint, HTML
- Best for: Management presentations and stakeholders

### Detailed Analysis
- Comprehensive technical breakdown
- Available formats: PDF, HTML, JSON
- Best for: SEO specialists and developers

## Scheduled Reports

### Frequency Options
- **Daily**: Automated reports every day at 9:00 AM
- **Weekly**: Reports every Monday at 9:00 AM
- **Monthly**: Reports on the first of each month at 9:00 AM

### Features
- **Email Integration**: Optional email delivery
- **Multiple Formats**: PDF, PowerPoint, HTML
- **Template Selection**: Choose from available templates
- **Management**: View and cancel active schedules

## Database Schema

The application uses SQLite for data persistence:

### Tables
- `seo_audits`: Individual audit results
- `competitor_analyses`: Competitor comparison data
- `seo_trends`: Historical trend data
- `scheduled_reports`: Automated report schedules

## Dependencies

### Core Dependencies
- `fastapi`: Web framework
- `uvicorn`: ASGI server
- `requests`: HTTP client
- `beautifulsoup4`: HTML parsing
- `python-dotenv`: Environment management

### Export Dependencies
- `reportlab`: PDF generation
- `python-pptx`: PowerPoint creation
- `jinja2`: HTML templating
- `schedule`: Automated task scheduling

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## License

This project is licensed under the MIT License.

## Support

For support and questions, please open an issue on GitHub. # Boostify
