# Tixoo - Modern Event Booking App

A premium mobile application built with Flutter, featuring a modern dark theme design inspired by industry-leading financial apps like CRED, CoinDCX, and Jupiter. This project focuses on providing a sleek and responsive interface for event discovery and browsing.

## ✨ Features

### 🎨 Modern Dark Theme Design
- **Deep dark backgrounds** with subtle gradients.
- **Clean contrast** and proper visual hierarchy.
- **Premium color palette** with accent colors.
- **Glassmorphism effects** and subtle shadows.

### 🧩 Scalable Component Structure
- **EventCard** - Reusable event listing component.
- **FeaturedBanner** - Hero banner with image overlays.
- **CategoryCard** - Interactive category selection.
- **ArtistCard** - Artist profile components.
- **SearchBarWidget** - Modern search with focus states.

### 🎭 Smooth Animations
- **Scale animations** on tap interactions.
- **Fade transitions** between screens.
- **Slide animations** for content reveal.
- **Focus animations** for search bar.

### 📱 Responsive Layout
- **Flexible grid system** for different screen sizes.
- **Adaptive spacing** and padding.
- **Scalable typography** hierarchy.
- **Touch-friendly** interactive elements.

## 🛠️ Framework Version Used

This project is developed using:
- **Flutter SDK**: `>=3.0.0 <4.0.0` (Compatible with Flutter 3.x.x stable releases)
- **Dart SDK**: `>=3.0.0 <4.0.0`

## 🖼️ Asset Setup

### Banner Images
1.  Create a folder named `images` inside `assets/`.
2.  Place your banner images (e.g., `banner_1.jpg`, `banner_2.jpg`, `banner_3.jpg`) inside `assets/images/`.
    *If these images are not present, the `FeaturedBanner` will display a placeholder.*

## 🚀 Getting Started

### Prerequisites
- Flutter SDK (>=3.0.0)
- Dart SDK
- Android Studio / VS Code with Flutter and Dart plugins

### Installation

1.  **Clone the repository**
    \`\`\`bash
    git clone <repository-url>
    cd tixoo_event_app
    \`\`\`

2.  **Install dependencies**
    Open your terminal in the project's root directory and run:
    \`\`\`bash
    flutter pub get
    \`\`\`

3.  **Ensure assets are in place**
    - (Optional) Add `banner_1.jpg`, `banner_2.jpg`, `banner_3.jpg` to `assets/images/` if you want to see the featured event banners.

4.  **Run the app**
    Connect a device or start an emulator, then run:
    \`\`\`bash
    flutter run
    \`\`\`

## 📐 App Structure

\`\`\`
lib/
├── main.dart                          # App entry point
├── theme/
│   └── app_theme.dart                 # Dark theme configuration
├── screens/
│   ├── splash_screen.dart             # Animated splash screen
│   └── events/
│       └── events_home_screen.dart    # Main events screen
└── widgets/
    └── events/
        ├── search_bar_widget.dart     # Search functionality
        ├── featured_banner.dart       # Hero banners
        ├── category_card.dart         # Category selection
        ├── event_card.dart            # Event listings
        └── artist_card.dart           # Artist profiles
└── assets/
    └── images/                        # Placeholder for banner images
\`\`\`

## 🎯 Key Sections

### Events Module
1.  **Header** - Time, location, notifications.
2.  **Search Bar** - Interactive search with animations.
3.  **Featured Events** - Swipeable banner carousel.
4.  **Categories** - Horizontal scrolling categories.
5.  **Upcoming Events** - Filterable event listings.
6.  **Artists** - Artist profiles with "See all" option.
7.  **Popular Events** - Trending event recommendations.

## 🎨 Design System

### Colors
- **Background**: `#0A0A0B` (Deep black)
- **Cards**: `#1A1A1C` (Dark gray)
- **Text Primary**: `#FFFFFF` (White)
- **Text Secondary**: `#9E9E9E` (Light gray)
- **Accent Blue**: `#007AFF`
- **Accent Purple**: `#8B5CF6`
- **Accent Orange**: `#FF9500`
- **Accent Green**: `#34C759`
- **Accent Pink**: `#FF2D92`
- **Error Color**: `#FF453A`

### Typography
- **Display**: 32px, Bold
- **Headline**: 22px, Bold
- **Title**: 16px, SemiBold
- **Body**: 14px, Regular
- **Caption**: 12px, Medium

### Spacing
- **Small**: 8px
- **Medium**: 16px
- **Large**: 24px
- **XLarge**: 32px

## 🔧 Customization

### Adding New Categories
Edit `_buildFeaturedCategories()` in `events_home_screen.dart`:

\`\`\`dart
final categories = [
  {'name': 'Music', 'icon': Icons.music_note, 'color': AppTheme.accentPurple},
  {'name': 'Your Category', 'icon': Icons.your_icon, 'color': AppTheme.yourColor},
];
\`\`\`

### Modifying Theme Colors
Update colors in `app_theme.dart`:

\`\`\`dart
static const Color yourCustomColor = Color(0xFF123456);
\`\`\`

## 📝 Notes on Challenges, Improvements, and Known Bugs

### Challenges
- **Static Data**: The event data displayed in the app (featured events, categories, upcoming events, artists) is currently static and hardcoded within the respective widgets or screens. This limits the dynamism of the content.

### Improvements
- **Real Event Data Integration**: Implement a real API service to fetch dynamic event data from a backend. This would involve using HTTP requests (e.g., with the `http` package or Dio) to retrieve event details, categories, and artist information.
- **Search Functionality**: Enhance the search bar to perform actual searches against dynamic event data, allowing users to find events based on keywords, location, or other criteria.
- **User Authentication & Event Booking**: Add user authentication to allow users to log in, save favorite events, and book tickets. This would require integrating with an authentication service (e.g., Firebase Auth, Supabase Auth).
- **Calendar Integration**: Allow users to add events directly to their device's calendar.
- **Push Notifications**: Implement push notifications for event reminders, updates, or new event announcements.
- **Location-Based Services**: Integrate location services to show nearby events or filter events by user's current location.
- **UI/UX Enhancements**: Further refine animations, add skeleton loaders for loading states when fetching real data, and implement pull-to-refresh for event lists.

### Known Bugs
- **Placeholder Images**: If banner images are not placed in `assets/images/`, the `FeaturedBanner` will display a generic placeholder, which might not be visually appealing.
- **No Data Persistence**: Since event data is static, there's no mechanism to persist user interactions (e.g., favoriting an event) or dynamically update event information without a real backend.

## 🤝 Contributing

1.  Fork the repository
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

-   Design inspiration from CRED, CoinDCX, and Jupiter
-   Flutter team for the amazing framework
-   Material Design guidelines
