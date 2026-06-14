# Pin Plan - Professional Fitness Cycle Tracker

A modern, feature-rich fitness cycle tracking application with AI diagnostics, comprehensive metrics tracking, and beautiful data visualizations.

## 🎯 Features

### Core Features
- **📊 Dashboard** - Real-time metrics overview with beautiful charts
- **🏋️ Training Tracker** - Log workouts with exercises, sets, reps, and weights
- **📈 Metrics Tracking** - Track weight, calories, macros, sleep, and mood
- **🔄 Cycle Management** - Create and manage training phases (bulk, cut, maintenance)
- **🎯 Goal Setting** - Set and track fitness goals with progress visualization
- **💡 AI Diagnostics** - Smart insights about your training and nutrition

### Data Visualization
- Weight trend charts
- Calorie intake tracking
- Macro distribution (protein, carbs, fats)
- Workout frequency and intensity
- Progress towards goals

### Local Storage
- **Persistent Data** - All data saves to browser localStorage (survives page refreshes and browser closes)
- **Export/Import** - Download your data as JSON or import from backup
- **No Server Required** - Complete privacy, your data never leaves your device

## 🚀 Getting Started

### Installation

1. **Clone or download this repository**

2. **Install dependencies:**
```bash
npm install
```

3. **Run development server:**
```bash
npm run dev
```

4. **Open browser:**
   - Navigate to `http://localhost:3000`

## 📋 How to Use

### Dashboard
- View your current stats and trends
- See active training cycle
- Log daily metrics directly from the dashboard
- Check AI-generated insights

### Metrics (Calories & Nutrition)
- Log daily nutrition data
- Track weight progression
- Filter data by time range (7, 30, 90 days)
- View historical metrics in a table

### Training (Workouts)
- Log individual workouts
- Track exercises with sets, reps, and weight
- Monitor workout duration and intensity
- View total volume and workout frequency

### Cycles (Training Phases)
- Create training phases (Bulk, Cut, Maintenance, Rest)
- Set target calories and protein per phase
- Track phase start and end dates
- View your active cycle status

### Goals
- Set short and long-term fitness goals
- Track progress with visual progress bars
- Update goal values as you progress
- See completed goals separately

### Data Management
- **Export Data**: Click the download icon to backup your data as JSON
- **Import Data**: Click the upload icon to restore from backup
- **Clear Data**: Delete specific entries from any tracker

## 🔧 Technical Stack

- **Framework**: Next.js 15
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Charts**: Recharts
- **Icons**: Lucide React
- **Storage**: Browser localStorage (100% client-side)

## 📱 Responsive Design

- Desktop optimized interface
- Mobile-friendly navigation
- Responsive charts and tables
- Touch-friendly buttons and controls

## 🎨 UI/UX Features

- **Modern Dark Theme** - Easy on the eyes for extended use
- **Smooth Animations** - Fade-in and slide-up effects
- **Intuitive Navigation** - Clear menu with active states
- **Real-time Updates** - Charts update instantly
- **Loading States** - Skeleton screens for smooth loading

## 🚀 Deployment to Vercel

### Step-by-Step Guide

1. **Push to GitHub:**
```bash
git init
git add .
git commit -m "Initial commit: Pin Plan 2.0"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/PinPlan.git
git push -u origin main
```

2. **Deploy on Vercel:**
   - Go to https://vercel.com
   - Click "New Project"
   - Select your GitHub repository
   - Vercel auto-detects Next.js
   - Click "Deploy"

3. **Done!** Your app is live

### Vercel Configuration

The `vercel.json` file is already configured with:
- Build command: `next build`
- Output directory: `.next`
- Install command: `npm install`

No additional setup needed!

## 📊 Data Structure

### LocalStorage Keys
- `pinplan_daily_metrics` - Daily nutrition and exercise data
- `pinplan_cycles` - Training phases
- `pinplan_goals` - Fitness goals
- `pinplan_workouts` - Detailed workout logs

## 🔒 Privacy & Security

- **100% Client-Side** - All data stored locally in your browser
- **No Server Tracking** - No analytics or data collection
- **Export Your Data** - Download anytime as JSON
- **Browser Storage** - Protected by your browser's security

## 💾 Backup Your Data

Regularly export your data:
1. Click the download icon in the navigation
2. Save the JSON file
3. Keep it safe

To restore:
1. Click the upload icon
2. Select your JSON backup file
3. Data is imported instantly

## 🎯 Recommended Usage

1. **Log daily metrics every evening** - Weight, calories, macros, sleep
2. **Log workouts during/after training** - Exercises, sets, reps
3. **Review dashboard weekly** - Check trends and insights
4. **Adjust phases quarterly** - Plan new training cycles
5. **Update goals monthly** - Track progress and celebrate wins

## 🐛 Troubleshooting

### Data Not Saving?
- Check browser localStorage settings
- Ensure cookies/storage is enabled
- Try a different browser
- Clear browser cache and reload

### Charts Not Showing?
- Need at least 2 data points
- Check that dates are in correct format
- Refresh the page

### Build Fails on Vercel?
- Check `package.json` syntax
- Verify all dependencies are listed
- Check for TypeScript errors: `npm run build` locally
- See Vercel build logs for details

## 📚 API Reference

### Storage Functions
```typescript
LocalStorage.addMetric(metric)
LocalStorage.getMetrics()
LocalStorage.updateMetric(id, updates)
LocalStorage.deleteMetric(id)

LocalStorage.addCycle(cycle)
LocalStorage.getCycles()
LocalStorage.getCurrentCycle()

LocalStorage.addGoal(goal)
LocalStorage.getGoals()
LocalStorage.updateGoal(id, updates)

LocalStorage.exportData()
LocalStorage.importData(data)
LocalStorage.clearAllData()
```

### Analytics Functions
```typescript
Analytics.getStatistics(days)
Analytics.generateInsights()
```

## 🚀 Future Enhancements

- Photo progress tracking
- Social sharing features
- Custom workout templates
- Macro calculator
- Advanced analytics and predictions
- Mobile app version
- Cloud sync option
- Community challenges

## 📝 License

This project is free to use and modify for personal use.

## 🤝 Support

For issues or questions:
1. Check this README
2. Review browser console for errors
3. Try exporting and importing data
4. Clear browser cache

## 🎉 Tips for Success

1. **Be Consistent** - Log data daily for best results
2. **Set Realistic Goals** - Adjust targets based on progress
3. **Review Weekly** - Check the dashboard for trends
4. **Backup Often** - Export data every week
5. **Experiment** - Try different training phases

---

**Pin Plan 2.0** - Built for serious fitness enthusiasts who want complete control over their training data. No ads, no tracking, no distractions. Just pure fitness tracking.

Happy training! 💪
