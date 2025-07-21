Tixoo – Modern Event Booking App
Tixoo is a premium event booking mobile application built with Flutter, inspired by modern fintech apps like CRED, CoinDCX, and Jupiter. It features a sleek dark theme, smooth animations, and a scalable UI system for browsing and discovering events in style.

✨ Features
🎨 Modern Dark Theme
Deep blacks with soft gradients

Premium contrast & visual hierarchy

Accent-driven color palette

Glassmorphism effects & subtle shadows

🧩 Scalable Component Structure
EventCard: Reusable listing tiles

FeaturedBanner: Hero banners with image overlays

CategoryCard: Event category selector

ArtistCard: Artist highlight widget

SearchBarWidget: Search with interactive focus states

🎭 Smooth Animations
Scale & fade effects on interactions

Screen transitions with slide and fade

Focus animations for input widgets

📱 Responsive Layout
Adaptive grid for all screen sizes

Touch-optimized layout

Scalable typography and flexible spacing

🔧 Tech Stack
Flutter SDK: >=3.0.0 <4.0.0

Dart SDK: >=3.0.0 <4.0.0

🖼️ Assets Setup
To show real banners:

Create folder: assets/images/

Add images:

Copy
Edit
banner_1.jpg  
banner_2.jpg  
banner_3.jpg  
If missing, a generic placeholder will be used.

🚀 Getting Started
📦 Prerequisites
Flutter SDK installed

Dart SDK installed

Code editor (VS Code / Android Studio)

🛠️ Installation
bash
Copy
Edit
git clone https://github.com/your_username/tixoo_event_app.git
cd tixoo_event_app
flutter pub get
flutter run
Ensure your device/emulator is connected and running.

📐 App Structure
bash
Copy
Edit
lib/
├── main.dart              # App entry point
├── theme/
│   └── app_theme.dart     # Theme config (dark mode, colors)
├── screens/
│   ├── splash_screen.dart
│   └── events/
│       └── events_home_screen.dart
└── widgets/
    └── events/
        ├── search_bar_widget.dart
        ├── featured_banner.dart
        ├── category_card.dart
        ├── event_card.dart
        └── artist_card.dart
assets/
└── images/                # Event banner assets
🎯 Key Modules
📍 Events Home Screen
Header – Displays date, location, and notification icon

Search – Animated search bar

Featured Events – Swipeable banner carousel

Categories – Horizontal scrollable cards

Upcoming Events – Filtered vertical listings

Artists – Top artists with “See all”

Popular Events – Highlighted trending events

🎨 Design System
🖌️ Colors
Element	Color
Background	#0A0A0B
Cards	#1A1A1C
Primary Text	#FFFFFF
Secondary Text	#9E9E9E
Accent Blue	#007AFF
Accent Purple	#8B5CF6
Accent Orange	#FF9500
Accent Green	#34C759
Accent Pink	#FF2D92
Error	#FF453A

🔤 Typography
Style	Size	Weight
Display	32px	Bold
Headline	22px	Bold
Title	16px	SemiBold
Body	14px	Regular
Caption	12px	Medium

📏 Spacing
Name	Size
Small	8px
Medium	16px
Large	24px
XLarge	32px

🧰 Customization Guide
➕ Add New Categories
Update _buildFeaturedCategories() in events_home_screen.dart:

dart
Copy
Edit
final categories = [
  {'name': 'Music', 'icon': Icons.music_note, 'color': AppTheme.accentPurple},
  {'name': 'Your Category', 'icon': Icons.your_icon, 'color': AppTheme.yourColor},
];
🎨 Change Theme Colors
Edit app_theme.dart:

dart
Copy
Edit
static const Color yourCustomColor = Color(0xFF123456);
🛠️ Improvements and Roadmap
⚠️ Known Issues
Static Data: All events are hardcoded.

No API / Real Data Integration.

No User State Persistence (like favorites or bookings).

No Real Authentication or Backend Support.

✅ Suggested Enhancements
Connect to REST API / Firebase for real-time event data

Implement full search filtering

Add User Authentication (Firebase / Supabase)

Enable Event Booking & Favorites

Integrate with Device Calendar

Add Push Notifications for event alerts

Use Geolocation to filter nearby events

Add Skeleton loaders and pull-to-refresh

🤝 Contributing
Fork the repository

Create a feature branch: git checkout -b feature/MyFeature

Commit your changes: git commit -m 'Add MyFeature'

Push the branch: git push origin feature/MyFeature

Open a Pull Request

📄 License
This project is licensed under the MIT License.
See the LICENSE file for more details.

🙏 Acknowledgments
Design inspiration: CRED, CoinDCX, Jupiter

Thanks to the Flutter Team for this amazing framework

Built with ❤️ following Material Design Guidelines

Let me know if you want me to:

Convert this into a .md file

Help push this to GitHub

Design a logo/banner

Add backend integration examples
