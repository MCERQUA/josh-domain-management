# Josh Domain Management

A comprehensive web application for managing Josh's portfolio of 553+ domains. This application provides a user-friendly interface for tracking, categorizing, and planning the development of a large domain portfolio.

## Project Overview

Josh (Contractors Choice Agency) owns a portfolio of 553+ domains primarily focused on insurance, construction trades, and geographic markets. This web application will serve as a central management tool to:

1. **Visualize the entire domain portfolio** with detailed categorization
2. **Track development status** of each domain
3. **Prioritize domains** for website development
4. **Search and filter domains** by various criteria
5. **Plan content and templates** for domain development
6. **Manage metadata** for each domain including SEO value, target audience, and business goals

## Technical Architecture

### Front-end
- **Framework**: Next.js with TypeScript
- **UI Library**: Tailwind CSS for styling
- **State Management**: React Context API with hooks
- **Data Visualization**: Chart.js for statistics and visualizations

### Back-end
- **Data Storage**: CSV/JSON files for domain data (with GitHub as the persistent storage)
- **API Routes**: Next.js API routes for data operations
- **Authentication**: Simple password protection (optional)

### Data Architecture
- **Domain Data**: Stored in CSV format for easy editing and viewing in spreadsheet applications
- **Category Definitions**: JSON format for hierarchical category structure
- **Status Tracking**: JSON format for development status tracking
- **Templates**: JSON format for template definitions and assignments

## Features

### 1. Dashboard
- Overview of domain portfolio with key statistics
- Quick filters for common views (Active, High Priority, By Category)
- Recent activity and updates
- Development progress visualization

### 2. Domain Explorer
- Comprehensive list view with sorting and filtering
- Detailed domain profile view
- Bulk operations for multiple domains
- Export functionality (CSV, Excel)

### 3. Search System
- Full-text search across all domain data
- Advanced filters by:
  - Category/Subcategory
  - Status
  - Priority
  - SEO Value
  - Keywords
  - Geographic focus
  - Industry/Niche

### 4. Category Management
- Hierarchical category structure
- Category statistics and metrics
- Ability to create/edit categories and assign domains

### 5. Development Planning
- Assign templates to domains
- Track development status
- Set priority levels
- Schedule development tasks
- Batch operations for similar domains

### 6. Template Management
- Define website templates
- Associate templates with categories
- Track template usage across domains

### 7. Import/Export System
- Import from GoDaddy or other domain registrars
- Batch update capabilities
- Export filtered sets of domains

## Data Structure

### Domain CSV Structure
The application will use a CSV file as the primary data source with the following fields:

```
domain_name,registration_date,expiration_date,category,subcategory,status,priority,seo_value,template,notes,target_audience,business_goals,keywords,geographic_focus,industry,hosting,forwarding_url,development_phase,last_updated
```

### JSON Category Structure
```json
{
  "categories": [
    {
      "id": "insurance",
      "name": "Insurance Industry",
      "subcategories": [
        {
          "id": "contractor_insurance",
          "name": "Contractor Insurance"
        },
        {
          "id": "specialty_vehicle",
          "name": "Specialty Vehicle Insurance"
        }
      ]
    },
    {
      "id": "construction",
      "name": "Construction & Trades",
      "subcategories": [
        {
          "id": "spray_foam",
          "name": "Spray Foam Industry"
        },
        {
          "id": "roofing",
          "name": "Roofing"
        }
      ]
    }
  ]
}
```

## Development Plan

### Phase 1: Foundation (1-2 weeks)
- Set up Next.js project with TypeScript and Tailwind CSS
- Create basic page structure and navigation
- Implement CSV parsing and data loading
- Create basic dashboard with stats

### Phase 2: Core Features (2-3 weeks)
- Implement domain explorer with filtering
- Build search functionality
- Create domain detail view
- Implement category management

### Phase 3: Advanced Features (2-3 weeks)
- Build template management system
- Implement development planning tools
- Create import/export functionality
- Add data visualization components

### Phase 4: Refinement (1-2 weeks)
- UI/UX improvements
- Performance optimization
- Bug fixes and testing
- Documentation

## Getting Started

This application will be built with simplicity and maintainability in mind. The data structure allows for easy updates via CSV files while providing powerful management capabilities through the web interface.

### Prerequisites
- Node.js 18+ (LTS)
- npm or yarn
- Git

### Setup and Installation
```bash
# Clone the repository
git clone https://github.com/MCERQUA/josh-domain-management.git

# Install dependencies
cd josh-domain-management
npm install

# Run the development server
npm run dev
```

### Data Management Workflow
1. Export domains from GoDaddy or other registrars
2. Process data into the required CSV format
3. Upload to the GitHub repository
4. Use the web interface for management and planning

## Contributing
This project is maintained by Echo Systems. For updates or feature requests, please contact the repository owner.

## License
This project is proprietary and owned by Echo Systems. All rights reserved.
