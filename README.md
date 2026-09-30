## el-backend
Base repository for app that brings together people with local foodtrucks and market stands.

# Eetlocal

> **Discover local vendors, wherever they are.**

Eetlocal is a mobile application designed to connect consumers with local market stalls, food trucks, market vendors and other independent local sellers.

The app aims to solve a simple problem:

**Consumers often don't know what local vendors are nearby, where they are trading, or when they will be there.**

Eetlocal brings this information together in one easy-to-use mobile experience.

---

## 🚧 Project Status

**Current stage:** MVP development

**Target:** Functional mobile MVP by the end of 2026

**Development approach:** Learn while building, using AI-assisted development where appropriate.

This project is currently being developed by the founders, with the architecture and codebase intentionally designed to allow experienced developers to contribute or take over development in the future.

---

# 🎯 Product Vision

Eetlocal aims to become a simple and reliable way for consumers to discover local vendors and for vendors to make their locations, schedules and products easier to discover.

The initial focus is on:

- Market stalls
- Food trucks
- Local food vendors
- Fresh produce sellers
- Independent local traders
- Other temporary/mobile vendors

The longer-term vision may expand beyond these categories as the product develops.

---

# 🧑‍🤝‍🧑 Target Users

## Consumers

People looking to discover local vendors, markets and food trucks.

Typical use cases include:

- Finding food trucks nearby
- Discovering local market stalls
- Finding fresh or locally produced products
- Checking where a particular vendor will be on a specific day
- Finding vendors while attending events or festivals
- Saving favourite vendors
- Reviewing vendors after visiting them

## Vendors

Independent vendors who operate from temporary, mobile or changing locations.

Typical use cases include:

- Creating a vendor profile
- Adding products/menu items
- Publishing locations
- Publishing dates and opening times
- Making their current availability visible
- Being discovered by nearby consumers
- Eventually receiving orders and analysing engagement

---

# 📱 MVP Scope

The first version of Eetlocal will focus on proving the core concept rather than implementing the complete long-term product vision.

## Consumer MVP

The consumer should be able to:

- Open the Eetlocal app
- Allow location access
- See nearby vendors
- View vendors on a map
- View vendors in a list
- Search/filter vendors
- Filter by date
- Filter by category
- View a vendor profile
- View vendor products/menu
- View vendor location and schedule
- Create an account
- Log in
- Save vendors as favourites
- Leave a basic review/rating

## Vendor MVP

A vendor should be able to:

- Create an account
- Log in
- Create/edit a vendor profile
- Add a description
- Add photos
- Add products/menu items
- Add trading locations
- Add dates and opening times
- Publish their availability
- Edit their information

---

# 🚫 Out of Scope for Initial MVP

The following features are part of the longer-term product vision but should **not** unnecessarily delay the first MVP:

- Online ordering
- Payments
- Delivery
- Complex vendor analytics
- Advanced recommendation engines
- AI recommendations
- Real-time moving vendor tracking
- Push notification systems
- Loyalty programmes
- Vendor subscriptions
- Advanced social features
- Complex event management
- Multi-language support
- Advanced review verification

These features can be evaluated after the initial MVP has been tested with real users.

---

# 🏗️ Technical Architecture

The initial application is planned around a simple, widely supported technology stack.

### Frontend

- **React Native**
- **Expo**
- **TypeScript**
- **Expo Router**

### Backend

- **Supabase**
- **PostgreSQL**
- **Supabase Authentication**
- **Supabase Storage**

### Development

- **GitHub**
- **VS Code**
- **Expo development tools**
- AI-assisted development

### Deployment

- **Expo EAS**
- Apple App Store
- Google Play Store

---

# 🧩 High-Level Architecture

```text
                    ┌─────────────────────┐
                    │     Eetlocal App    │
                    │                     │
                    │ React Native        │
                    │ Expo                │
                    │ TypeScript          │
                    └──────────┬──────────┘
                               │
                               │
                    ┌──────────▼──────────┐
                    │      Supabase       │
                    │                     │
                    │ Authentication      │
                    │ API                 │
                    │ Storage             │
                    │ Security            │
                    └──────────┬──────────┘
                               │
                    ┌──────────▼──────────┐
                    │     PostgreSQL      │
                    │                     │
                    │ Users               │
                    │ Vendors             │
                    │ Locations           │
                    │ Products            │
                    │ Schedules           │
                    │ Favourites          │
                    │ Reviews             │
                    └─────────────────────┘
