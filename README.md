🌱 My Farm — Smart Farm Manager

AI-Powered Multi-Tenant Android App for Precision Agriculture & Farm Operations

📖 Overview

My Farm is a production-grade, enterprise-class Android application built to empower farmers and agricultural managers with real-time intelligence, multi-year recordkeeping, and multimodal AI advisory. Operating with an offline-first architecture, it provides robust data durability, tenant isolation, and seamless cloud synchronization.

Whether tracking daily irrigation cycles, diagnosing crop leaf pathology via computer vision, mapping field plot boundaries using Google Maps satellite layers, or analyzing multi-year profit and loss statements, My Farm brings modern SaaS capabilities directly into the hands of growers.

✨ Key Features

🤖 Gemini 3.5 AI Agronomist: Context-aware AI assistant grounded in your actual database records (crops, historical yields, transactions, weather). Includes multilingual support (English, Marathi, Hindi) and voice input.

🛰️ Satellite Weather & NDVI Intelligence: Real-time numerical weather forecasts via Open-Meteo, complete with automated agricultural alerts, foliar spraying window advisories, and Sentinel-2 satellite NDVI biomass data.

🗺️ Interactive Google Maps Boundary Tracer: Draw polygons around field plots, calculate precise acreage and hectares geodesically, and search locations via native geocoding.

🌾 Multi-Year Crop & Field Lifecycle Tracking: Manage multiple plots, track growth stages (from sowing to harvest), log inputs, and preserve multi-year seasonal archives (2024–2026).

🩺 Multimodal Crop Disease Scanner: Upload plant photographs or describe symptoms to receive instant AI pathology diagnosis, confidence scores, safe immediate actions (IPM), and expert consultation triggers.

💰 Financial Accounting & P&L Ledger: Track crop sales income, seed/fertilizer/labor expenses, and calculate net returns in INR with seasonal breakdowns.

📄 Professional Vector PDF Report Generator: Compile multi-page printable PDF reports for banking loans, Krishi Vigyan Kendra (KVK) consultations, or personal archives using native Android canvas rendering.

🔒 Secure Multi-Tenant Authentication: Tenant session management, SHA-256 password hashing with application salting, token-based password recovery, and platform admin audit logging.

🛠️ Tech Stack & Architecture

UI Framework: Jetpack Compose with Material 3 design system and custom agricultural color palette.

Architecture Pattern: MVVM (Model-View-ViewModel) with unidirectional data flow using Kotlin Coroutines and Flows.

Local Persistence: Android Room SQLite Database with foreign-key relationships, offline durability, and automatic migrations.

Networking: Retrofit 2 with Moshi JSON converter and OkHttp logging interceptors.

Location & Maps: Google Play Services Location & Maps Compose SDK (maps-compose).

Testing: Comprehensive unit tests, instrumented tests, and Robolectric test suites.

🚀 Getting Started Locally

Prerequisites

Android Studio: Ladybug, Koala, or newer.

Android SDK: API Level 36 (Android 14/15+) installed via SDK Manager.

JDK: Java 11 or higher.

Installation Steps

Clone or download the repository to your local machine.

Open Android Studio, select Open, and choose the project root directory.

Allow Gradle to sync dependencies automatically.

Create a .env file in the root directory (refer to .env.example) and add your API keys:

GEMINI_API_KEY=your_gemini_api_key_here
MAPS_API_KEY=your_google_maps_api_key_here


Connect a physical Android device (with USB Debugging enabled) or start an AVD Emulator (API 24+).

Click Run 'app' (Shift + F10) in Android Studio.

💡 Quick Demo Mode

If you want to explore the app instantly without setting up external accounts:

On the login screen, tap the "Explore Demo Account (Sample Data)" button to load pre-populated farms, active plots, multi-year crop records, and financial ledgers.

📄 License

Distributed under the MIT License. See LICENSE for more information.
