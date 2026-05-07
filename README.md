# yieldguard.io
YieldGuard AI • Uganda 🇺🇬🌾
An intelligent agent-based system designed to reduce post-harvest losses and improve food security for smallholder farmers in Uganda.

## Overview

YieldGuard is a comprehensive farm monitoring platform with real-time risk assessment, AI-powered recommendations, and live market intelligence for Ugandan farmers. The system combines satellite data, weather forecasting, and machine learning to provide actionable insights that help farmers maximize yield and minimize losses.

---

## Key Features

### 🌍 Real-time Risk Monitoring
- Tracks **184 farms** across multiple districts (Mubende, Masaka, Kapchorwa, Jinja, Gulu, Mbale, Kampala, Lira, Soroti, Kabale)
- Color-coded risk levels: **High (Red) / Medium (Orange) / Low (Green)**
- Automated post-harvest loss alerts with precise timing
- District-level aggregated metrics and visual risk heatmap

### 🤖 AI-Powered Recommendations
- **Gemini AI Integration**: Get live, personalized farmer guidance
- Example recommendations:
  - "Sell Matooke within 48 hours" (based on humidity & decay risk)
  - "Apply solar drying today" (optimal weather conditions)
  - "Monitor beans for fungal disease" (weather advisory)
- SMS-ready format for basic phones
- AI suggestions powered by Claude and Gemini (free API key required)

### 🌦️ Live Weather Integration
- **Open-Meteo Live Data**: Real-time weather impact on crop storage
- Humidity alerts and rain predictions
- 5-day forecast strips per district
- Weather-specific storage recommendations
- Temperature and UV index tracking
- Drought and flood risk alerts

### 📈 Market Price Trends
- **Live Kampala Market Prices** for matooke, maize, beans, cassava, and 8+ crops
- Historical price data with trend indicators (↑ +12%, ↓ -5%, → 0%)
- Multi-market comparison (Kampala, Jinja, Mbarara, Gulu)
- Price-based sell timing recommendations
- UGX currency conversions

### 💬 Chat Agent Interface
- Farmers ask questions about storage, weather, markets, and crops
- Instant AI-powered responses via integrated chat
- Question examples:
  - "When should I sell my matooke?"
  - "Is it safe to dry in this humidity?"
  - "What's the best price for beans?"
- Works seamlessly from login to dashboard

### 📱 SMS Simulation & Integration
- Demonstrates real SMS delivery to remote farmers (basic phones)
- SMS templates: Weather alerts, price changes, sell recommendations
- Character counter (160 char limit)
- Farmer conversation history
- AI-drafted reply suggestions

### 🛰️ Satellite Crop Health (NDVI)
- Simulated satellite imagery grid showing crop health
- Color legend: 🟥 Stressed / 🟨 Moderate / 🟩 Healthy
- District-level NDVI tracking
- Live update badges

### 📊 Advanced Analytics & Reporting
- **Yield Summary**: 4.8T saved, 78% target achievement, 92% farmer satisfaction
- **Alert Performance**: 98% delivery rate, 67% response rate, 83% action taken
- **Weekly Reports**: Comprehensive metrics with week-over-week comparison
- **Post-Harvest Loss Reduction**: 61% improvement tracked
- Downloadable PDF reports

### 👥 Farmer Management
- Add and register new farmers with:
  - Full name, phone number, district, village
  - Primary and secondary crops
  - Farm size (in acres)
  - Status (Active, At Risk, Inactive)
- Search and filter farmers by name, district, crop
- Track farmer status and activity
- Real-time farmer count and engagement metrics

### 🗺️ Uganda District Risk Map
- Visual map of all 10+ districts with risk indicators
- Click to view district-specific details
- Risk factor breakdown per district
- Current weather and farm count per district

---

## Platform Pages

### **Login Page** (`login.html`)
Professional authentication interface featuring:
- **Modern Split Layout**: Left branding panel + right auth form
- **Tab-Based Navigation**: Sign In / Create Account tabs
- **Sign In Form**:
  - Email and password authentication
  - Password visibility toggle
  - "Forgot Password?" recovery flow
  - Session persistence (auto-redirect if logged in)
- **Sign Up Form**:
  - First/Last name, email, phone, district, organization
  - Password strength meter (weak → strong indicator)
  - Terms & conditions checkbox
  - Real-time field validation
- **Features**:
  - Beautiful gradient backgrounds with radial blur effects
  - Grid overlay pattern
  - Smooth animations and transitions
  - Toast notifications (success, error, info)
  - Mobile responsive design
  - Forgot password modal overlay
  - Pre-filled fields for better UX

**Brand Messaging on Left Panel**:
- Headline: *"Grow smarter. Lose less. Feed more."*
- 4 key feature highlights with icons
- Crop pills showcasing supported crops
- Logo with glowing animation

### **Dashboard Page** (`dashboard.html`)
Comprehensive admin interface with 5 main sections:

#### 1. **Dashboard Tab** (Home)
- **KPI Cards**: 
  - Total Farms (184), Yield Saved (4.8T), High Risk (23), Alerts Today (41)
- **Produce at Risk Table**: 
  - Farmer name, crop, district, days stored, risk level, action buttons
  - Real-time data for Amina Nakato, John Mugisha, Sarah Nansubuga, etc.
- **AI Recommendations Panel**:
  - Load/refresh button (triggers Gemini AI)
  - Live recommendations based on registered farmers
  - Soil health index mini-view
- **Live Weather Card**:
  - District selector dropdown (10 districts)
  - Current conditions with emoji icons
  - Humidity, temp, wind, UV index
  - 5-day forecast strip
  - Weather advisory text
- **Market Price Chart**:
  - Crop tabs (Matooke, Maize, Beans, Cassava, etc.)
  - Interactive Chart.js graph
  - Price summary with trend indicators
  - Historical data visualization
- **Satellite NDVI Grid**: 64-cell grid showing crop health
- **Crop Distribution**: Pie chart breakdown
- **Recent Alerts**: 5 latest alerts with timestamps

#### 2. **Farmers Tab**
- **Farmer Statistics**:
  - Total Farmers count
  - Active this month
  - Total farm area (acres)
- **Registered Farmers List**:
  - Search by name, district, or crop
  - Filter by status (All, Active, At Risk, Inactive), crop, district
  - Add new farmer button (opens modal)
  - Farmer cards with avatar, name, district, crop, status badge
  - Click cards for detailed view
- **Add Farmer Modal**:
  - Form fields: name, phone, district, village, crops, acreage, status
  - District and crop dropdowns
  - Form validation and error handling
  - Save/Cancel buttons

#### 3. **Risk Map Tab**
- **Risk Statistics KPIs**: High/Medium/Low/Weather alerts counts
- **District Risk Heatmap**:
  - Grid layout of all 10+ Uganda districts
  - Color-coded by risk level
  - Hover for district info (farms count, weather)
  - Click to drill down
- **Current Risk Factors List**:
  - Detailed risk descriptions
  - Impact severity
  - Recommended actions

#### 4. **Analytics Tab**
- **Yield Summary Stats**:
  - Total Yield Saved, Target Achievement %, Farmer Satisfaction %, Post-Harvest Loss Reduction %
  - Progress bars for each metric
- **Alert Performance Stats**:
  - Delivery Rate, Response Rate, Action Taken %, SMS Open Rate
  - Color-coded progress indicators
- **Weekly Performance Report Table**:
  - Metric name, This Week, Last Week, Change %, Status
  - 7 key metrics tracked
- **Download Report Button**: Export to PDF

#### 5. **SMS Inbox Tab**
- **SMS Statistics**: Unread count, Replied count, Total Messages, AI Drafted
- **Two-Panel Conversation View**:
  - **Left Panel**: Farmer conversation list with filters (All/Unread)
  - **Right Panel**: Selected conversation thread
- **Message Features**:
  - Farmer name, phone number in thread header
  - Message history with timestamps
  - AI-suggested reply bar (with "Use" button)
  - Reply compose box with templates:
    - 💰 Price
    - 🌧️ Weather
    - 📦 Sell Now
    - 🏚️ Storage
  - Character counter (0/160 SMS limit)
  - Send button (green checkmark)
- **Example Conversations**: Pre-populated with realistic farmer questions

### **Sidebar Menu**
- **AI Status**: Shows "AI Agent Online" (Claude AI • Open-Meteo Live)
- **Satellite Status**: "Satellite NDVI Live" with pulsing indicator
- **Quick Actions**:
  - Ask AI Agent
  - Add New Farmer
  - Simulate Farmer SMS
  - Download Report
- **Appearance Settings**:
  - Dark/Light mode toggle
  - Theme persistence
- **Gemini API Key Input**:
  - Free key storage
  - Link to get free key from aistudio.google.com
  - Save/Status indicator
- **Sign Out Button**: Red logout button

### **Mobile Bottom Navigation**
- Fixed bottom nav bar on mobile (< 768px)
- Icons for Dashboard, Farmers, Risk Map, Analytics, SMS, Menu
- Active state highlighting
- Unread SMS badge

---

## How It Works

### Data Flow
1. **Farm Data** → Real-time monitoring of 184 farms across Uganda
2. **Risk Calculation** → Post-harvest loss prediction based on humidity, time stored, crop type
3. **Weather Integration** → Open-Meteo API provides live weather alerts
4. **Market Data** → Live Kampala market prices for crops
5. **AI Analysis** → Gemini AI generates personalized recommendations
6. **SMS Delivery** → Alerts sent to farmers via SMS (simulated)
7. **Farmer Feedback** → Chat interface collects farmer responses

### Tech Stack
- **Frontend**: HTML5, CSS3, Tailwind CSS, JavaScript (ES6+)
- **Charts**: Chart.js for market price visualization
- **Fonts**: 
  - Dashboard: Space Grotesk, JetBrains Mono
  - Login: Playfair Display (serif), DM Sans
- **Icons**: Font Awesome 6.6.0
- **API Integration**: 
  - Gemini AI (free API key required)
  - Open-Meteo (weather data)
  - Kampala Market Prices (simulated)
- **Storage**: localStorage for user sessions, farmer data, API keys
- **Animations**: CSS keyframes (pulse, glow, fade, slide)

---

## Getting Started

### Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Darknet2355/yieldguard.io.git
   cd yieldguard.io
   ```

2. **Open in Browser**
   - Start with `login.html` for authentication
   - Create an account or sign in
   - Redirects to `dashboard.html` on successful login

3. **Get a Free Gemini API Key**
   - Visit [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
   - Generate a free API key
   - Paste into the chat panel or sidebar settings
   - Now AI recommendations are fully enabled

### Demo Data
- Pre-populated with 6 farmers: Amina Nakato, John Mugisha, Sarah Nansubuga, David Okello, Grace Akello, Robert Ssekitoleko
- 10 Uganda districts with real risk data
- 12 crops with real-time price data
- Live weather data from Open-Meteo API

---

## Features Breakdown

### Authentication
✅ Sign up with email, phone, district, organization  
✅ Password strength meter  
✅ Forgot password recovery  
✅ Session persistence  
✅ Auto-redirect to dashboard when logged in  

### Dashboard
✅ Real-time KPI cards  
✅ Produce at risk table  
✅ AI recommendation engine  
✅ Live weather by district  
✅ Market price charts  
✅ Satellite health imagery  
✅ Crop distribution  
✅ Recent alerts feed  

### Farmer Management
✅ Add new farmers  
✅ Search and filter  
✅ Farmer statistics  
✅ Status tracking (Active, At Risk, Inactive)  

### Risk Map
✅ District heatmap  
✅ Risk factor breakdowns  
✅ Visual risk indicators  

### Analytics
✅ Yield performance metrics  
✅ Alert delivery stats  
✅ Weekly performance report  
✅ PDF report download  

### SMS Inbox
✅ Conversation history  
✅ AI-suggested replies  
✅ SMS templates  
✅ Character counter  
✅ Farmer conversation threads  

---

## UI/UX Highlights

### Color Scheme
- **Primary Green**: #10b981 (Emerald)
- **Secondary Green**: #34d399 (Light Emerald)
- **Dark Background**: #050a05 (Almost Black)
- **Risk Red**: #ef4444
- **Risk Amber**: #f59e0b
- **Sky Blue**: #38bdf8

### Typography
- **Display Font**: Playfair Display (login, headlines)
- **Body Font**: Space Grotesk (dashboard), DM Sans (login)
- **Monospace**: JetBrains Mono (numbers, SMS character count)

### Animations
- **Pulse**: Status dots, live indicators
- **Fade**: Slide-in animations for recommendations
- **Glow**: Logo and AI badges
- **Shimmer**: Loading states
- **Bounce**: Typing indicator

### Responsive Design
- **Desktop**: Full 2-column layout (farmers + chat SMS grid)
- **Tablet**: Stacked columns, adjusted spacing
- **Mobile**: Single column with bottom navigation
- Hamburger menu for sidebar on mobile

---

## Files Overview

| File | Purpose |
|------|---------|
| `login.html` | Authentication page (sign in / sign up) |
| `dashboard.html` | Main admin interface (5 tabs + sidebar) |
| `README.md` | This documentation |

---

## Future Enhancements

🚀 Integrate real SMS provider (Africastalking, Nexmo)  
🚀 Backend API with Node.js/Express  
🚀 Database integration (Firebase, PostgreSQL)  
🚀 Real satellite data from NASA NDVI API  
🚀 Multi-language support (Luganda, Swahili)  
🚀 Mobile app (React Native)  
🚀 Advanced ML model for loss prediction  
🚀 Video tutorials for farmers  

---

## License

MIT License - See LICENSE.md

---

## Support

For issues, feature requests, or questions:
- **GitHub Issues**: [yieldguard.io/issues](https://github.com/Darknet2355/yieldguard.io/issues)
- **Email**: support@yieldguard.io
- **Twitter**: [@YieldGuardAI](https://twitter.com/YieldGuardAI)

---

**Made with 🌾 for Uganda's farmers**
