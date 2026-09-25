# Dawago 💊

Dawago is a modern, mobile-first online pharmacy frontend designed for local Indian customers.

The goal is to create a simple and trustworthy experience where customers can:

- Search for medicines
- Browse medicine categories
- View medicine details
- Add medicines to cart
- Upload a prescription
- Place a mock order
- Track orders
- View previous orders
- Manage their profile

This is currently a **frontend-only prototype**.

DO NOT implement a backend, database, authentication, real payments, real prescription processing, or external APIs.

All data should use realistic mock data.

---

# Product Vision

Dawago is designed around a simple idea:

> "Your local pharmacy, now online."

The experience should feel:

- Trustworthy
- Clean
- Fast
- Modern
- Local
- Mobile-first
- Easy enough for non-technical users

Dawago should NOT look like a generic ecommerce website.

It should feel like a healthcare/pharmacy product.

---

# Technology

Use:

- Next.js
- TypeScript
- React
- Tailwind CSS
- shadcn/ui
- Lucide React icons

Do not introduce additional frameworks unless absolutely necessary.

---

# Development Rules

## Frontend only

Do NOT create:

- Backend APIs
- Database
- Authentication system
- Payment integration
- Real prescription processing
- External healthcare APIs
- Real delivery tracking

Use mock data.

All interactions should work visually using React state.

---

# Design Direction

Create a premium but approachable Indian healthcare UI.

The design should be:

- Clean
- Spacious
- Modern
- Friendly
- Trustworthy
- Accessible

Avoid excessive gradients.

Avoid excessive animations.

Avoid overly rounded "AI startup" aesthetics.

Avoid copying Tata 1mg's exact UI.

Dawago should have its own visual identity.

---

# Brand

## Name

Dawago

## Tagline

"Your local pharmacy, now online."

Alternative supporting text:

"Medicines delivered from a pharmacy you can trust."

---

# Color System

Use a healthcare-inspired visual system.

Primary:

- Deep green
- Fresh green

Secondary:

- White
- Very light green
- Soft gray

Accent:

- Warm yellow/orange for offers

Text:

- Dark charcoal
- Medium gray

Use Tailwind classes rather than hardcoded CSS wherever possible.

Create reusable color tokens where appropriate.

---

# Typography

Use a clean modern sans-serif font.

Prioritize readability.

Headings should be bold but not oversized.

Body text should be comfortable to read on mobile.

---

# Responsive Design

The application must be mobile-first.

Primary target:

Mobile phones

Secondary:

Tablet

Desktop

The website should work at:

- 360px
- 390px
- 430px
- 768px
- 1024px
- 1440px

---

# Application Structure

Create these pages:

/                 → Home

/search           → Search medicines

/medicine/[id]    → Medicine details

/categories      → Medicine categories

/cart             → Shopping cart

/checkout         → Checkout

/orders           → Orders

/orders/[id]      → Order details

/profile           → Customer profile

/prescription      → Upload prescription

/pharmacy          → Pharmacy dashboard

/pharmacy/orders   → Pharmacy orders

/pharmacy/inventory → Pharmacy inventory

---

# Navigation

## Desktop

Top navigation:

Dawago logo

Search bar

Categories

Orders

Profile

Cart

Example:

--------------------------------------------------

DAWAGO

[ 🔍 Search medicines, brands, or conditions ]

Categories   Orders   Profile   🛒 Cart

--------------------------------------------------

## Mobile

Use a sticky bottom navigation:

Home

Categories

Orders

Profile

Cart

The search bar should remain highly visible on the home screen.

---

# Home Page

The home page is the most important page.

Create the following sections.

---

## 1. Header

Desktop:

Dawago logo

Location

Search

Orders

Profile

Cart

Mobile:

Dawago logo

Location

Cart

Search below header

---

## 2. Location

Display:

"Delivering to"

"Sarjapur, Bangalore"

Use mock location data.

Allow the user to visually change location, but do not implement actual GPS.

---

## 3. Main Search

Large search box:

"Search medicines, brands or health products"

Include search icon.

When clicked, navigate to:

/search

Example searches:

- Paracetamol
- Cetirizine
- Pantoprazole
- Vitamin D
- ORS

---

# 4. Prescription CTA

Create a highly visible card.

Example:

-----------------------------------------

📋 Have a prescription?

Upload your prescription and we'll help
you find the medicines.

[ Upload Prescription ]

-----------------------------------------

The button should navigate to:

/prescription

For now, clicking upload should simulate the interface only.

---

# 5. Categories

Create horizontally scrollable categories on mobile.

Categories:

Pain Relief

Cold & Cough

Diabetes

Heart Care

Vitamins

Digestive Health

Skin Care

Personal Care

Baby Care

First Aid

Each category should have:

- Icon
- Name

Use Lucide icons where appropriate.

---

# 6. Popular Medicines

Create a horizontal scrolling medicine card section on mobile.

Example medicines:

Paracetamol 650mg

Cetirizine 10mg

Pantoprazole 40mg

ORS Sachet

Vitamin D3

Azithromycin 500mg

Each card should contain:

- Medicine name
- Generic name
- Pack size
- Price
- MRP
- Discount
- Add button

Example:

Paracetamol 650mg

10 tablets

₹28

MRP ₹35

20% OFF

[ + Add ]

---

# 7. Offers Banner

Create a promotional banner.

Example:

"Save on your everyday medicines"

"Free delivery on orders above ₹499"

[ Shop Now ]

Use mock promotional data.

---

# 8. Why Dawago?

Create a section with four cards:

✓ Trusted local pharmacy

✓ Genuine medicines

✓ Local delivery

✓ Pharmacist support

---

# 9. Recently Purchased

If mock customer data exists, display:

"Buy Again"

Example:

Paracetamol 650mg

Cetirizine 10mg

Pantoprazole 40mg

Each should have:

[ Buy Again ]

---

# 10. Footer

Include:

Dawago

Your local pharmacy, now online.

Links:

About

Contact

Privacy

Terms

Help

Pharmacy

Copyright Dawago

---

# Search Page

Create:

Large search bar

Filters

Search results

Sort options

Example:

Search:

"paracetamol"

Results:

24 medicines found

Filters:

Category

Price

Brand

Form

Prescription required

Sort:

Relevance

Price: Low to High

Price: High to Low

---

# Medicine Card

Every medicine card should include:

- Medicine image placeholder
- Medicine name
- Generic name
- Strength
- Manufacturer
- Pack size
- MRP
- Selling price
- Discount
- Prescription indicator if applicable
- Add button

Example:

--------------------------------

Paracetamol 650mg

Paracetamol

10 tablets

₹28

MRP ₹35

20% OFF

[ + Add ]

--------------------------------

---

# Medicine Details Page

Create a clean product details page.

Show:

Medicine name

Generic name

Manufacturer

Strength

Dosage form

Pack size

MRP

Selling price

Discount

Availability

Prescription requirement

Description

Important information

---

## Product Actions

Quantity selector

[ Add to Cart ]

[ Buy Now ]

---

# Prescription Notice

If a medicine requires prescription:

Display a noticeable warning:

"Prescription required"

And:

"You will need to provide a valid prescription before this medicine can be dispensed."

Do not implement medical advice.

---

# Cart Page

Display:

Cart items

Quantity controls

Remove button

Subtotal

Delivery fee

Discount

Total

Example:

--------------------------------

Your Cart

Paracetamol 650mg

₹28

[-] 2 [+]

₹56

--------------------------------

Subtotal ₹56

Delivery ₹30

Total ₹86

[ Proceed to Checkout ]

---

# Checkout Page

Create a clean checkout flow.

Sections:

1. Delivery address

2. Order summary

3. Delivery fee

4. Payment method

For now payment should be MOCK ONLY.

Options:

Cash on Delivery

UPI

Card

When user clicks:

"Place Order"

create a mock order in React state/localStorage.

Navigate to:

/orders/[id]

---

# Prescription Page

Create a professional prescription upload UI.

Title:

"Upload your prescription"

Subtitle:

"Upload a clear photo or PDF of your prescription."

Upload area:

--------------------------------

📷

Drag and drop your prescription

or

[ Choose File ]

Supported:

JPG, PNG, PDF

Maximum size:

10MB

--------------------------------

After selecting a file:

Show file name

Show preview for images

Button:

[ Continue ]

Since this is frontend-only, simulate successful upload.

Display:

"Prescription uploaded successfully."

---

# Orders Page

Display:

"My Orders"

Tabs:

All

Processing

Out for Delivery

Delivered

Cancelled

Example order:

--------------------------------

Order #DWA1024

Placed on 25 Sep 2026

₹420

3 items

Status:

Out for delivery

[ View Order ]

--------------------------------

---

# Order Details Page

Display:

Order number

Order date

Order status

Items

Delivery address

Payment method

Total

Timeline:

Order placed

↓

Pharmacy confirmed

↓

Being packed

↓

Out for delivery

↓

Delivered

Use a clean visual timeline.

---

# Profile Page

Display:

Profile information

Name

Phone

Email

Saved addresses

Orders

Help

Privacy

Terms

Logout

---

# Pharmacy Dashboard

Create a separate pharmacy interface.

This is a frontend prototype for the pharmacy owner.

Desktop dashboard layout:

Sidebar

Dashboard

Orders

Inventory

Prescriptions

Customers

Settings

Main content

---

# Pharmacy Dashboard Home

Show statistics:

Today's Orders

Pending Orders

Completed Orders

Today's Revenue

Example:

Today's Orders

24

Pending

7

Completed

17

Revenue

₹18,450

---

# Recent Orders

Table:

Order ID

Customer

Items

Amount

Status

Date

Actions

Example:

DWA1024

Rahul Sharma

3 items

₹420

Pending

25 Sep

[ View ]

---

# Pharmacy Orders

Create order management interface.

Filters:

All

New

Processing

Ready

Out for Delivery

Completed

Cancelled

Each order should have:

Order ID

Customer

Items

Prescription indicator

Amount

Status

Time

Action button

---

# Pharmacy Order Details

Display:

Customer information

Order items

Prescription

Order amount

Delivery address

Order status

Buttons:

[ Accept Order ]

[ Reject Order ]

[ Mark as Packing ]

[ Mark Ready ]

[ Assign Delivery ]

[ Mark Delivered ]

These buttons only change frontend state.

---

# Pharmacy Inventory

Create an inventory table.

Columns:

Medicine

Generic Name

Stock

Price

MRP

Expiry

Status

Actions

Example:

Paracetamol 650mg

Paracetamol

42

₹28

₹35

Dec 2027

In Stock

[ Edit ]

---

# Inventory Status

Use:

In Stock

Low Stock

Out of Stock

Example:

42 → In Stock

5 → Low Stock

0 → Out of Stock

---

# Mock Data

Create a dedicated mock data file.

Example:

/src/data/medicines.ts

Include at least 30 medicines.

Use realistic Indian pharmacy products.

Example:

Paracetamol 650mg

Cetirizine 10mg

Pantoprazole 40mg

ORS

Vitamin D3

Azithromycin 500mg

Amoxicillin 500mg

Ibuprofen 400mg

Antacid tablets

Multivitamin tablets

Do not provide medical recommendations.

The data exists only to demonstrate the UI.

---

# State Management

For the frontend prototype use:

React state

and/or

localStorage

for:

- Cart
- Mock orders
- Recently viewed medicines
- Selected address
- UI preferences

Do not add Redux unless the application actually requires it.

---

# Components

Create reusable components.

Suggested structure:

src/

components/

Navbar.tsx

MobileBottomNav.tsx

SearchBar.tsx

MedicineCard.tsx

CategoryCard.tsx

PrescriptionUpload.tsx

OfferBanner.tsx

CartItem.tsx

OrderCard.tsx

OrderTimeline.tsx

PharmacySidebar.tsx

StatsCard.tsx

InventoryTable.tsx

Footer.tsx

---

# UX Requirements

The website must feel fast.

Use loading skeletons where appropriate.

Use hover states on desktop.

Use touch-friendly buttons on mobile.

Buttons should have obvious visual feedback.

Avoid tiny clickable elements.

Use clear empty states.

Example empty cart:

"Your cart is empty"

"Find medicines for your everyday needs."

[ Browse Medicines ]

---

# Accessibility

Use:

- Semantic HTML
- Accessible buttons
- Proper labels
- Keyboard navigation
- Sufficient contrast
- Alt text for images
- ARIA labels where appropriate

---

# Error States

Create frontend error states.

Examples:

Search:

"No medicines found."

Cart:

"Your cart is empty."

Prescription:

"File type not supported."

Orders:

"No orders yet."

---

# Loading States

Create skeleton loading components for:

Medicine cards

Orders

Dashboard statistics

Inventory

---

# Animations

Use subtle animations only.

Examples:

- Button hover
- Card hover
- Cart item added
- Page transitions
- Modal opening

Do NOT use excessive animations.

The app should feel fast.

---

# Images

For now use:

- Placeholder medicine images
- Generic pharmacy imagery
- Icons

Do not scrape images from other pharmacy websites.

---

# Important Medical Safety Rule

This is a pharmacy commerce interface.

The application must NOT:

- Diagnose users
- Recommend prescription medicines
- Recommend medication doses
- Replace a pharmacist or doctor
- Automatically approve prescriptions

The frontend may display medicine information purely as product/catalogue information.

---

# Important Development Rule

Build one page at a time.

Do not generate the entire application in one massive component.

Start with:

1. Global layout
2. Navbar
3. Home page
4. Medicine cards
5. Search page
6. Medicine details
7. Cart
8. Checkout
9. Prescription page
10. Orders
11. Profile
12. Pharmacy dashboard

After completing each major section, ensure the application still builds successfully.

---

# Code Quality

Use:

- TypeScript types
- Reusable components
- Clean folder structure
- Small components
- Meaningful variable names
- No unnecessary duplication
- No hardcoded secrets

Avoid:

- `any` unless absolutely necessary
- giant components
- duplicated UI
- inline styles where Tailwind can be used
- unnecessary dependencies

---

# Final Goal

The final frontend should feel like a real production-ready pharmacy website even though all backend functionality is mocked.

The customer should be able to navigate this complete flow:

Home

↓

Search medicine

↓

Medicine details

↓

Add to cart

↓

Cart

↓

Checkout

↓

Mock order created

↓

Order details

↓

Order tracking

The pharmacy owner should be able to navigate:

Pharmacy Dashboard

↓

Orders

↓

Order details

↓

Inventory

↓

Prescription interface

All functionality is simulated locally for now.

---

# Future Roadmap

Do NOT implement these yet.

Future versions may add:

- Supabase database
- Customer authentication
- Pharmacy authentication
- Real inventory
- Prescription storage
- Pharmacist verification
- Payment gateway
- WhatsApp notifications
- SMS notifications
- Delivery management
- Multiple pharmacies
- Location-based pharmacy search
- Order tracking
- Analytics
- Android application
- iOS application
- ABDM integration

The current objective is only:

> Build a beautiful, fast and convincing frontend prototype for Dawago.
