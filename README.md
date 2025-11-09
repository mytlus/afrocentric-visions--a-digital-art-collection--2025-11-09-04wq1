# Afrocentric Visions Landing Page - Maintenance & Customization Guide

A comprehensive guide for maintaining, updating, and customizing the Afrocentric Visions landing page. This guide is designed for beginners with little to no coding experience.

---

## Table of Contents

1. [Getting Started](#getting-started)
2. [Updating Text Content](#updating-text-content)
3. [Modifying Tailwind CSS Classes](#modifying-tailwind-css-classes)
4. [Fixing and Managing Links](#fixing-and-managing-links)
5. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
6. [Troubleshooting Guide](#troubleshooting-guide)
7. [Best Practices](#best-practices)

---

## Getting Started

### What You'll Need

- **A text editor**: Programs like Visual Studio Code (free), Notepad++, or even basic Notepad
- **A web browser**: Chrome, Firefox, Safari, or Edge to preview your changes
- **The HTML file**: The `index.html` file provided
- **Basic understanding**: This guide assumes no prior coding experience

### How to Edit the File

1. **Open the HTML file** in your text editor (right-click the file → "Open with" → choose your text editor)
2. **Make your changes** following the instructions in this guide
3. **Save the file** using Ctrl+S (Windows) or Cmd+S (Mac)
4. **Preview changes** by opening the file in your web browser (double-click the HTML file)
5. **Refresh the browser** (press F5 or Ctrl+R) to see your latest changes

### File Structure Overview

The landing page is organized into these main sections:

```
index.html
├── Announcement Bar (shipping notification)
├── Header Navigation (logo, menu, search)
├── Hero Section (main banner with large image)
├── Features Section (3 feature cards)
├── Benefits Section (3 benefit blocks with images)
├── About Us Section (company story and values)
├── Testimonials Section (customer reviews)
├── FAQ Section (frequently asked questions)
├── CTA Section (call-to-action)
├── Contact Section (contact form and info)
├── Footer (links, social media, newsletter)
└── JavaScript (interactive features)
```

---

## Updating Text Content

### Understanding the HTML Structure

HTML uses **tags** (commands) to structure content. Tags look like this: `<tagname>content</tagname>`

**Common tags you'll encounter:**
- `<h1>`, `<h2>`, `<h3>` = Headings (h1 is largest, h3 is smaller)
- `<p>` = Paragraph text
- `<a>` = Links
- `<button>` = Buttons
- `<span>` = Small text container

**Example:**
```html
<h1>This is a heading</h1>
<p>This is paragraph text</p>
```

### Updating Text in Different Sections

#### 1. **Announcement Bar** (Top notification)

**Location**: Line ~43 in the HTML

**Current text:**
```html
<p class="flex items-center justify-center gap-2">
    <i class="fas fa-truck"></i>
    Fast Worldwide Shipping (5 days delivery)
</p>
```

**How to change it:**
- Find the text "Fast Worldwide Shipping (5 days delivery)"
- Replace it with your message
- Keep the `<i class="fas fa-truck"></i>` part (this is the truck icon)

**Example - Change to:**
```html
<p class="flex items-center justify-center gap-2">
    <i class="fas fa-truck"></i>
    Free Shipping on Orders Over $100
</p>
```

#### 2. **Header Logo and Brand Name** (Top left corner)

**Location**: Line ~54-58

**Current code:**
```html
<div class="flex items-center gap-2">
    <i class="fas fa-palette text-2xl text-amber-700"></i>
    <span class="text-2xl font-bold text-gray-900 tracking-tight">Afrocentric Visions</span>
</div>
```

**How to change the brand name:**
- Find `Afrocentric Visions`
- Replace with your brand name
- Keep the icon and styling

**Example:**
```html
<span class="text-2xl font-bold text-gray-900 tracking-tight">Your Brand Name</span>
```

#### 3. **Hero Section Main Headline**

**Location**: Line ~115-119

**Current text:**
```html
<h1 class="text-4xl md:text-6xl font-bold text-white mb-6 tracking-tight leading-tight">
    Afrocentric Visions: A Digital Art Collection
</h1>
```

**How to change it:**
- Replace the text between the `<h1>` tags
- Keep all the `class` information (it controls styling)

**Example:**
```html
<h1 class="text-4xl md:text-6xl font-bold text-white mb-6 tracking-tight leading-tight">
    Your New Headline Here
</h1>
```

#### 4. **Hero Section Subheadline**

**Location**: Line ~120-123

**Current text:**
```html
<p class="text-xl md:text-2xl text-gray-100 mb-8 leading-relaxed">
    Immerse yourself in a curated gallery of stunning Afrocentric digital art that celebrates culture, creativity, and connection.
</p>
```

**How to change it:**
```html
<p class="text-xl md:text-2xl text-gray-100 mb-8 leading-relaxed">
    Your new subheadline text goes here
</p>
```

#### 5. **Features Section Title and Description**

**Location**: Line ~150-156

**Current code:**
```html
<h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-4 tracking-tight">
    Premium Digital Art Features
</h2>
<p class="text-xl text-gray-600 max-w-2xl mx-auto">
    Discover what makes our Afrocentric art collection exceptional and perfect for your space.
</p>
```

**How to update:**
```html
<h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-4 tracking-tight">
    Your Feature Title
</h2>
<p class="text-xl text-gray-600 max-w-2xl mx-auto">
    Your feature description
</p>
```

#### 6. **Individual Feature Cards**

**Location**: Line ~164-180 (Feature 1), Line ~182-198 (Feature 2), Line ~200-216 (Feature 3)

**Example - Feature 1 Card:**
```html
<div class="bg-white border border-gray-200 rounded-xl p-8 transition-smooth hover-lift hover:shadow-xl hover:border-amber-700">
    <div class="bg-amber-100 w-16 h-16 rounded-lg flex items-center justify-center mb-6">
        <i class="fas fa-image text-amber-700 text-2xl"></i>
    </div>
    <h3 class="text-2xl font-bold text-gray-900 mb-3">Digital Prints</h3>
    <p class="text-gray-600 leading-relaxed mb-4">
        High-resolution digital artwork available for instant download. Perfect for personal projects, presentations, and creative endeavors.
    </p>
    <ul class="space-y-2 text-sm text-gray-600">
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-amber-700"></i>
            4K Resolution
        </li>
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-amber-700"></i>
            Multiple Formats
        </li>
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-amber-700"></i>
            Instant Access
        </li>
    </ul>
</div>
```

**To update this card:**

1. **Change the title** (Digital Prints):
```html
<h3 class="text-2xl font-bold text-gray-900 mb-3">Your New Title</h3>
```

2. **Change the description**:
```html
<p class="text-gray-600 leading-relaxed mb-4">
    Your new description text here
</p>
```

3. **Change the bullet points**:
```html
<li class="flex items-center gap-2">
    <i class="fas fa-check text-amber-700"></i>
    Your new bullet point
</li>
```

4. **Change the icon** (optional):
   - Find `<i class="fas fa-image text-amber-700 text-2xl"></i>`
   - Replace `fa-image` with another icon name
   - See [Font Awesome Icons List](https://fontawesome.com/icons) for options
   - Example: `fa-download`, `fa-star`, `fa-heart`

#### 7. **Benefits Section**

**Location**: Line ~230-390

Each benefit has a title, description, and bullet points. Here's how to update them:

**Example - Benefit 1 Title:**
```html
<h3 class="text-3xl font-bold text-gray-900 mb-4">Transforming Digital Spaces</h3>
```

**Change to:**
```html
<h3 class="text-3xl font-bold text-gray-900 mb-4">Your New Benefit Title</h3>
```

**Update the description:**
```html
<p class="text-gray-600 text-lg leading-relaxed mb-6">
    Your new benefit description goes here. Make it compelling and descriptive.
</p>
```

**Update benefit bullet points:**
```html
<div class="flex items-start gap-4">
    <i class="fas fa-star text-amber-700 text-xl mt-1"></i>
    <div>
        <h4 class="font-semibold text-gray-900">Your Benefit Title</h4>
        <p class="text-gray-600 text-sm">Your benefit description</p>
    </div>
</div>
```

#### 8. **About Us Section**

**Location**: Line ~410-480

**Update the "Our Story" section:**
```html
<h3 class="text-2xl font-bold text-gray-900 mb-6 flex items-center gap-3">
    <i class="fas fa-history text-amber-700"></i>
    Our Story
</h3>
<p class="text-gray-700 leading-relaxed text-lg">
    Replace this paragraph with your company's story
</p>
```

**Update the "Our Mission" section:**
```html
<h3 class="text-2xl font-bold text-gray-900 mb-6 flex items-center gap-3">
    <i class="fas fa-compass text-amber-700"></i>
    Our Mission
</h3>
<p class="text-gray-700 leading-relaxed text-lg">
    Replace this paragraph with your company's mission
</p>
```

**Update Core Values:**
```html
<div>
    <i class="fas fa-palette text-4xl mb-4"></i>
    <h4 class="font-bold mb-2">Authenticity</h4>
    <p class="text-amber-100">Your value description here</p>
</div>
```

#### 9. **Testimonials Section**

**Location**: Line ~520-610

**Example - Update a testimonial:**
```html
<div class="bg-white rounded-xl p-8 shadow-md transition-smooth hover-lift hover:shadow-lg border border-gray-200">
    <div class="flex items-center gap-1 mb-4">
        <i class="fas fa-star text-amber-700"></i>
        <i class="fas fa-star text-amber-700"></i>
        <i class="fas fa-star text-amber-700"></i>
        <i class="fas fa-star text-amber-700"></i>
        <i class="fas fa-star text-amber-700"></i>
    </div>
    <p class="text-gray-700 leading-relaxed mb-6 text-lg">
        "Your testimonial text goes here. Include the customer's experience and positive feedback."
    </p>
    <div class="flex items-center gap-4">
        <div class="w-12 h-12 bg-gradient-to-br from-amber-400 to-orange-500 rounded-full flex items-center justify-center text-white font-bold">
            AK
        </div>
        <div>
            <p class="font-bold text-gray-900">Customer Name</p>
            <p class="text-sm text-gray-600">Job Title, City</p>
        </div>
    </div>
</div>
```

**To customize:**
- Replace the testimonial text in quotes
- Change the initials (AK) to match the customer name
- Update customer name and location

#### 10. **FAQ Section**

**Location**: Line ~630-720

**Example - Update an FAQ item:**
```html
<div class="faq-item">
    <button class="faq-toggle w-full text-left py-6 px-6 bg-gray-50 hover:bg-gray-100 rounded-lg transition-smooth flex items-center justify-between font-semibold text-lg text-gray-900">
        <span>What file formats are available for digital prints?</span>
        <i class="fas fa-chevron-down text-amber-700"></i>
    </button>
    <div class="faq-answer px-6 pb-6">
        <p class="text-gray-700 leading-relaxed">
            Your answer text goes here. Provide detailed, helpful information.
        </p>
    </div>
</div>
```

**To update:**
1. Change the question text (between the `<span>` tags)
2. Change the answer text (between the `<p>` tags in the faq-answer div)

#### 11. **Contact Information**

**Location**: Line ~800-830

**Update email address:**
```html
<a href="mailto:1stdigitalartistry@gmail.com" class="text-amber-700 hover:text-amber-800 transition-smooth font-semibold">
    1stdigitalartistry@gmail.com
</a>
```

**Change to your email:**
```html
<a href="mailto:your@email.com" class="text-amber-700 hover:text-amber-800 transition-smooth font-semibold">
    your@email.com
</a>
```

**Update business hours:**
```html
<p class="mt-2 text-gray-600">
    Monday - Friday: 9:00 AM - 6:00 PM EST<br>
    Saturday - Sunday: 10:00 AM - 4:00 PM EST
</p>
```

#### 12. **Footer Copyright Year**

**Location**: Line ~1020

The year automatically updates using JavaScript, but you can customize the footer text:

```html
<p class="mb-2">
    &copy; <span id="year"></span> Afrocentric Visions. All rights reserved. | 
    <a href="privacy.html" class="text-amber-700 hover:text-amber-600 transition-smooth">Privacy Policy</a> | 
    <a href="terms.html" class="text-amber-700 hover:text-amber-600 transition-smooth">Terms of Service</a>
</p>
```

**Change company name in footer:**
```html
&copy; <span id="year"></span> Your Company Name. All rights reserved. |
```

#### 13. **Footer Company Description**

**Location**: Line ~960-970

```html
<p class="text-gray-400 leading-relaxed mb-6">
    Celebrating African creativity through a curated collection of premium digital art and framed prints.
</p>
```

**Update to your description:**
```html
<p class="text-gray-400 leading-relaxed mb-6">
    Your company description goes here. Keep it brief and compelling.
</p>
```

---

## Modifying Tailwind CSS Classes

### What is Tailwind CSS?

Tailwind CSS is a system of pre-made styling instructions. Instead of writing complex CSS code, you add class names to HTML elements to style them.

**Example:**
```html
<!-- This creates a button that's amber-colored, bold, and has padding -->
<button class="bg-amber-700 hover:bg-amber-800 text-white px-6 py-2 rounded-lg font-semibold">
    Click Me
</button>
```

### Common Tailwind Classes Used on This Page

#### **Colors**

The page uses a color scheme with amber and orange tones. Here's what each color class does:

| Class | Purpose | Example |
|-------|---------|---------|
| `text-amber-700` | Text color (dark amber) | `<p class="text-amber-700">Text</p>` |
| `bg-amber-700` | Background color (dark amber) | `<div class="bg-amber-700">Box</div>` |
| `text-white` | White text | `<p class="text-white">Text</p>` |
| `text-gray-900` | Dark gray text | `<p class="text-gray-900">Text</p>` |
| `bg-gray-50` | Light gray background | `<div class="bg-gray-50">Box</div>` |
| `hover:text-amber-700` | Change color on hover | `<a class="hover:text-amber-700">Link</a>` |

**Color options** (you can replace numbers):
- `50, 100, 200, 300, 400, 500, 600, 700, 800, 900`
- Higher numbers = darker
- Example: `text-gray-900` is very dark, `text-gray-100` is very light

#### **Spacing (Padding & Margins)**

- `px-4` = Horizontal padding (left and right)
- `py-4` = Vertical padding (top and bottom)
- `p-8` = Padding on all sides
- `mb-6` = Margin bottom
- `gap-4` = Space between items

**Number scale:** `0, 1, 2, 3, 4, 6, 8, 12, 16, 20, 24, 32`

#### **Typography (Text Styling)**

- `text-lg` = Large text
- `text-2xl` = Extra large text
- `text-4xl` = Very large text (headlines)
- `font-bold` = Bold text
- `font-semibold` = Semi-bold text
- `leading-relaxed` = More space between lines

#### **Sizing**

- `w-full` = Full width
- `h-screen` = Full height of screen
- `rounded-lg` = Slightly rounded corners
- `rounded-xl` = More rounded corners
- `shadow-lg` = Large shadow effect

#### **Responsive Design**

Classes with prefixes control how things look on different screen sizes:

- `md:` = Medium screens (tablets)
- `lg:` = Large screens (desktops)

**Example:**
```html
<h1 class="text-4xl md:text-6xl">
    This is 4xl on phones, but 6xl on tablets and larger
</h1>
```

### How to Change Colors

**Task: Change the primary color from amber to blue**

1. **Find all amber color classes** in the HTML
2. **Replace them with blue classes**

**Common replacements:**
```html
<!-- Before (Amber) -->
<button class="bg-amber-700 hover:bg-amber-800 text-white">

<!-- After (Blue) -->
<button class="bg-blue-700 hover:bg-blue-800 text-white">
```

**All amber colors used on this page:**
- `text-amber-700` → `text-blue-700`
- `bg-amber-700` → `bg-blue-700`
- `hover:bg-amber-800` → `hover:bg-blue-800`
- `bg-amber-100` → `bg-blue-100`
- `hover:text-amber-700` → `hover:text-blue-700`
- `hover:border-amber-700` → `hover:border-blue-700`
- `focus:border-amber-700` → `focus:border-blue-700`
- `text-amber-50` → `text-blue-50`
- `text-amber-900` → `text-blue-900`
- `focus:ring-amber-200` → `focus:ring-blue-200`

**Available color families:**
- `blue`, `purple`, `pink`, `red`, `orange`, `yellow`, `green`, `teal`, `cyan`, `indigo`, `violet`

### How to Change Spacing

**Task: Add more space between sections**

Current spacing between sections:
```html
<section class="py-24">
```

This means 24 units of padding on top and bottom.

**To increase spacing:**
```html
<section class="py-32">  <!-- More space -->
```

**To decrease spacing:**
```html
<section class="py-16">  <!-- Less space -->
```

**Spacing scale:** `0, 1, 2, 3, 4, 6, 8, 12, 16, 20, 24, 28, 32, 36, 40, 44, 48, 52, 56, 60, 64, 72, 80, 96`

### How to Change Text Sizes

**Task: Make the hero headline smaller**

Current:
```html
<h1 class="text-4xl md:text-6xl">
```

**To make smaller:**
```html
<h1 class="text-3xl md:text-5xl">
```

**Text size scale:** `xs, sm, base, lg, xl, 2xl, 3xl, 4xl, 5xl, 6xl, 7xl, 8xl, 9xl`

### How to Change Border Radius (Rounded Corners)

**Current rounded corners:**
```html
<div class="rounded-xl">
```

**Options:**
- `rounded-none` = No rounding
- `rounded-sm` = Slight rounding
- `rounded-lg` = Medium rounding
- `rounded-xl` = More rounding
- `rounded-2xl` = Even more rounding
- `rounded-full` = Completely round (circle)

### How to Change Shadows

**Current shadow:**
```html
<div class="shadow-lg">
```

**Options:**
- `shadow-sm` = Tiny shadow
- `shadow-md` = Medium shadow
- `shadow-lg` = Large shadow
- `shadow-xl` = Extra large shadow
- `shadow-2xl` = Huge shadow

### How to Change Button Styling

**Current button:**
```html
<button class="bg-amber-700 hover:bg-amber-800 text-white px-8 py-4 rounded-lg font-bold text-lg transition-smooth hover:scale-105 transform duration-300 shadow-lg hover:shadow-xl">
    Shop Now
</button>
```

**To make button larger:**
- Change `px-8 py-4` to `px-10 py-5`

**To make button smaller:**
- Change `px-8 py-4` to `px-6 py-3`

**To make button text smaller:**
- Change `text-lg` to `text-base` or `text-sm`

**To remove the "grow on hover" effect:**
- Remove `hover:scale-105 transform`

### How to Change Grid Layout

**Current 3-column grid (Features section):**
```html
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
```

**This means:**
- `grid-cols-1` = 1 column on phones
- `md:grid-cols-3` = 3 columns on tablets and larger
- `gap-8` = 8 units of space between items

**To change to 2 columns on tablets:**
```html
<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
```

**To add 4 columns on large screens:**
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
```

### How to Change Container Width

**Current container:**
```html
<div class="container mx-auto px-4 max-w-7xl">
```

- `max-w-7xl` = Maximum width of 80rem (1280px)

**To make narrower:**
```html
<div class="container mx-auto px-4 max-w-4xl">
```

**Width options:** `max-w-xs, max-w-sm, max-w-md, max-w-lg, max-w-xl, max-w-2xl, max-w-3xl, max-w-4xl, max-w-5xl, max-w-6xl, max-w-7xl`

---

## Fixing and Managing Links

### Understanding Links in HTML

A link is created using the `<a>` tag:

```html
<a href="https://example.com">Click Here</a>
```

**Parts of a link:**
- `<a>` = Link tag
- `href="..."` = Where the link goes
- `Click Here` = Text that appears on the page
- `</a>` = Closing tag

### Types of Links

#### **1. External Links** (Link to another website)
```html
<a href="https://www.example.com">Visit Example</a>
```

#### **2. Internal Links** (Link to a section on the same page)
```html
<a href="#features">Go to Features</a>
```

#### **3. Email Links**
```html
<a href="mailto:your@email.com">Email Us</a>
```

#### **4. Phone Links**
```html
<a href="tel:+1234567890">Call Us</a>
```

### Finding All Links on This Page

Here's where all the important links are located:

#### **Navigation Menu Links** (Line ~60-67)

**Desktop menu:**
```html
<a href="#home" class="text-gray-700 hover:text-amber-700 transition-smooth font-medium">Home</a>
<a href="#features" class="text-gray-700 hover:text-amber-700 transition-smooth font-medium">Features</a>
<a href="#benefits" class="text-gray-700 hover:text-amber-700 transition-smooth font-medium">Benefits</a>
<a href="#about" class="text-gray-700 hover:text-amber-700 transition-smooth font-medium">About</a>
<a href="#testimonials" class="text-gray-700 hover:text-amber-700 transition-smooth font-medium">Testimonials</a>
<a href="#faq" class="text-gray-700 hover:text-amber-700 transition-smooth font-medium">FAQ</a>
<a href="#contact" class="text-gray-700 hover:text-amber-700 transition-smooth font-medium">Contact</a>
```

**Mobile menu** (Line ~91-97) - Same links, repeated for mobile

These are **internal links** that scroll to sections on the same page. They should work correctly without changes.

#### **"Shop Now" Buttons** (Multiple locations)

**Header button** (Line ~73):
```html
<button class="bg-amber-700 hover:bg-amber-800 text-white px-6 py-2 rounded-lg font-semibold transition-smooth hover:scale-105 transform">
    Shop Now
</button>
```

**Hero section buttons** (Line ~124-130):
```html
<button class="bg-amber-700 hover:bg-amber-800 text-white px-8 py-4 rounded-lg font-bold text-lg transition-smooth hover:scale-105 transform duration-300 shadow-lg hover:shadow-xl">
    Explore Collection
</button>
<button class="bg-white hover:bg-gray-100 text-amber-700 px-8 py-4 rounded-lg font-bold text-lg transition-smooth hover:scale-105 transform duration-300 shadow-lg hover:shadow-xl">
    Learn More
</button>
```

**CTA section buttons** (Line ~750-755):
```html
<button class="bg-white hover:bg-gray-100 text-amber-700 px-8 py-4 rounded-lg font-bold text-lg transition-smooth hover:scale-105 transform duration-300 shadow-lg hover:shadow-xl">
    Shop Collection
</button>
<button class="bg-amber-900 hover:bg-amber-950 text-white px-8 py-4 rounded-lg font-bold text-lg transition-smooth hover:scale-105 transform duration-300 shadow-lg hover:shadow-xl border-2 border-white">
    Learn More
</button>
```

**⚠️ Important:** These buttons currently don't go anywhere. They need to be converted to links or connected to your shopping platform.

#### **Contact Email Link** (Line ~810)

```html
<a href="mailto:1stdigitalartistry@gmail.com" class="text-amber-700 hover:text-amber-800 transition-smooth font-semibold">
    1stdigitalartistry@gmail.com
</a>
```

**How to change email:**
```html
<a href="mailto:your@email.com" class="text-amber-700 hover:text-amber-800 transition-smooth font-semibold">
    your@email.com
</a>
```

#### **Footer Links** (Line ~950-1020)

**Quick Links section:**
```html
<a href="#home" class="text-gray-400 hover:text-amber-700 transition-smooth">Home</a>
<a href="#features" class="text-gray-400 hover:text-amber-700 transition-smooth">Features</a>
<a href="#benefits" class="text-gray-400 hover:text-amber-700 transition-smooth">Benefits</a>
<a href="#about" class="text-gray-400 hover:text-amber-700 transition-smooth">About Us</a>
<a href="#contact" class="text-gray-400 hover:text-amber-700 transition-smooth">Contact</a>
```

**Collections section** (Line ~975-980):
```html
<a href="#" class="text-gray-400 hover:text-amber-700 transition-smooth">Digital Prints</a>
<a href="#" class="text-gray-400 hover:text-amber-700 transition-smooth">Framed Art</a>
<a href="#" class="text-gray-400 hover:text-amber-700 transition-smooth">Limited Editions</a>
<a href="#" class="text-gray-400 hover:text-amber-700 transition-smooth">Artist Collaborations</a>
<a href="#" class="text-gray-400 hover:text-amber-700 transition-smooth">New Releases</a>
```

**⚠️ These use `href="#"` which means they don't go anywhere yet.**

**Support & Info section** (Line ~982-987):
```html
<a href="privacy.html" class="text-gray-400 hover:text-amber-700 transition-smooth">Privacy Policy</a>
<a href="terms.html" class="text-gray-400 hover:text-amber-700 transition-smooth">Terms of Service</a>
<a href="blog.html" class="text-gray-400 hover:text-amber-700 transition-smooth">Blog</a>
<a href="#" class="text-gray-400 hover:text-amber-700 transition-smooth">FAQ</a>
<a href="#contact" class="text-gray-400 hover:text-amber-700 transition-smooth">Contact Us</a>
```

**Footer bottom links** (Line ~1022-1025):
```html
<a href="privacy.html" class="text-amber-700 hover:text-amber-600 transition-smooth">Privacy Policy</a> | 
<a href="terms.html" class="text-amber-700 hover:text-amber-600 transition-smooth">Terms of Service</a>
```

**Social media links** (Line ~938-950):
```html
<a href="#" class="w-10 h-10 bg-gray-800 hover:bg-amber-700 rounded-full flex items-center justify-center transition-smooth">
    <i class="fab fa-facebook-f text-white"></i>
</a>
```

### Step-by-Step: Updating Links

#### **Step 1: Update Collection Links**

**Current code** (Line ~975-980):
```html
<a href="#" class="text-gray-400 hover:text-amber-700 transition-smooth">Digital Prints</a>
<a href="#" class="text-gray-400 hover:text-amber-700 transition-smooth">Framed Art</a>
<a href="#" class="text-gray-400 hover:text-amber-700 transition-smooth">Limited Editions</a>
<a href="#" class="text-gray-400 hover:text-amber-700 transition-smooth">Artist Collaborations</a>
<a href="#" class="text-gray-400 hover:text-amber-700 transition-smooth">New Releases</a>
```

**Updated with real links:**
```html
<a href="https://yourshop.com/digital-prints" class="text-gray-400 hover:text-amber-700 transition-smooth">Digital Prints</a>
<a href="https://yourshop.com/framed-art" class="text-gray-400 hover:text-amber-700 transition-smooth">Framed Art</a>
<a href="https://yourshop.com/limited-editions" class="text-gray-400 hover:text-amber-700 transition-smooth">Limited Editions</a>
<a href="https://yourshop.com/collaborations" class="text-gray-400 hover:text-amber-700 transition-smooth">Artist Collaborations</a>
<a href="https://yourshop.com/new-releases" class="text-gray-400 hover:text-amber-700 transition-smooth">New Releases</a>
```

#### **Step 2: Update Social Media Links**

**Current code** (Line ~938-950):
```html
<a href="#" class="w-10 h-10 bg-gray-800 hover:bg-amber-700 rounded-full flex items-center justify-center transition-smooth">
    <i class="fab fa-facebook-f text-white"></i>
</a>
<a href="#" class="w-10 h-10 bg-gray-800 hover:bg-amber-700 rounded-full flex items-center justify-center transition-smooth">
    <i class="fab fa-instagram text-white"></i>
</a>
<a href="#" class="w-10 h-10 bg-gray-800 hover:bg-amber-700 rounded-full flex items-center justify-center transition-smooth">
    <i class="fab fa-twitter text-white"></i>
</a>
<a href="#" class="w-10 h-10 bg-gray-800 hover:bg-amber-700 rounded-full flex items-center justify-center transition-smooth">
    <i class="fab fa-pinterest text-white"></i>
</a>
```

**Updated with real social media links:**
```html
<a href="https://www.facebook.com/yourpage" class="w-10 h-10 bg-gray-800 hover:bg-amber-700 rounded-full flex items-center justify-center transition-smooth">
    <i class="fab fa-facebook-f text-white"></i>
</a>
<a href="https://www.instagram.com/yourprofile" class="w-10 h-10 bg-gray-800 hover:bg-amber-700 rounded-full flex items-center justify-center transition-smooth">
    <i class="fab fa-instagram text-white"></i>
</a>
<a href="https://www.twitter.com/yourprofile" class="w-10 h-10 bg-gray-800 hover:bg-amber-700 rounded-full flex items-center justify-center transition-smooth">
    <i class="fab fa-twitter text-white"></i>
</a>
<a href="https://www.pinterest.com/yourprofile" class="w-10 h-10 bg-gray-800 hover:bg-amber-700 rounded-full flex items-center justify-center transition-smooth">
    <i class="fab fa-pinterest text-white"></i>
</a>
```

#### **Step 3: Convert "Shop Now" Buttons to Links**

**Current button** (Line ~73):
```html
<button class="bg-amber-700 hover:bg-amber-800 text-white px-6 py-2 rounded-lg font-semibold transition-smooth hover:scale-105 transform">
    Shop Now
</button>
```

**Convert to a link that looks like a button:**
```html
<a href="https://yourshop.com" class="inline-block bg-amber-700 hover:bg-amber-800 text-white px-6 py-2 rounded-lg font-semibold transition-smooth hover:scale-105 transform">
    Shop Now
</a>
```

**Key change:** Replace `<button>` with `<a href="...">` and add `inline-block` class

**Repeat for all "Shop Now" buttons:**

Hero section (Line ~124-130):
```html
<a href="https://yourshop.com/explore" class="inline-block bg-amber-700 hover:bg-amber-800 text-white px-8 py-4 rounded-lg font-bold text-lg transition-smooth hover:scale-105 transform duration-300 shadow-lg hover:shadow-xl">
    Explore Collection
</a>
<a href="https://yourshop.com/learn-more" class="inline-block bg-white hover:bg-gray-100 text-amber-700 px-8 py-4 rounded-lg font-bold text-lg transition-smooth hover:scale-105 transform duration-300 shadow-lg hover:shadow-xl">
    Learn More
</a>
```

CTA section (Line ~750-755):
```html
<a href="https://yourshop.com/shop" class="inline-block bg-white hover:bg-gray-100 text-amber-700 px-8 py-4 rounded-lg font-bold text-lg transition-smooth hover:scale-105 transform duration-300 shadow-lg hover:shadow-xl">
    Shop Collection
</a>
<a href="https://yourshop.com/learn" class="inline-block bg-amber-900 hover:bg-amber-950 text-white px-8 py-4 rounded-lg font-bold text-lg transition-smooth hover:scale-105 transform duration-300 shadow-lg hover:shadow-xl border-2 border-white">
    Learn More
</a>
```

#### **Step 4: Update Contact Form Action**

**Current form** (Line ~835):
```html
<form class="space-y-6">
```

**To send emails, update to:**
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" class="space-y-6">
```

**To get a form ID:**
1. Go to [Formspree.io](https://formspree.io)
2. Sign up for free
3. Create a new form
4. Copy the form ID
5. Replace `YOUR_FORM_ID` with your actual ID

### Common Link Mistakes to Avoid

| ❌ Mistake | ✅ Correct | Problem |
|-----------|----------|---------|
| `href="www.example.com"` | `href="https://www.example.com"` | Missing protocol |
| `href="page.html#section"` | `href="page.html#section"` | Inconsistent paths |
| `href="contact.html"` | `href="./contact.html"` | Wrong relative path |
| `href="#"` | `href="https://..."` | Link goes nowhere |
| `href="Contact"` | `href="#contact"` | Wrong section ID format |

### Testing Your Links

**How to check if links work:**

1. **Save your HTML file** (Ctrl+S or Cmd+S)
2. **Open it in your browser** (double-click the file)
3. **Click each link** to verify it works
4. **Check the browser address bar** to confirm the URL is correct

**If a link doesn't work:**
- Check that the URL is spelled correctly
- Make sure it starts with `https://` for external links
- For internal links, verify the section ID matches (e.g., `#contact` must match `id="contact"`)

---

## Adding Privacy and Terms Pages

### Understanding Why You Need These Pages

- **Privacy Policy**: Tells visitors how you collect and use their data
- **Terms of Service**: Explains the rules for using your website and products

These are legal documents that protect your business and inform customers.

### Method 1: Create Simple Privacy and Terms Pages

#### **Step 1: Create the Privacy Policy File**

1. **Open your text editor**
2. **Create a new file** (File → New)
3. **Paste this code:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy - Afrocentric Visions">
    <title>Privacy Policy - Afrocentric Visions</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-white text-gray-900 font-sans">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="container mx-auto px-4 py-4 max-w-7xl">
            <div class="flex items-center justify-between">
                <div class="flex items-center gap-2">
                    <i class="fas fa-palette text-2xl text-amber-700"></i>
                    <a href="index.html" class="text-2xl font-bold text-gray-900 tracking-tight hover:text-amber-700 transition-smooth">Afrocentric Visions</a>
                </div>
                <a href="index.html" class="text-gray-700 hover:text-amber-700 transition-smooth font-medium">Back to Home</a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-24 bg-white">
        <div class="container mx-auto px-4 max-w-4xl">
            <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8 tracking-tight">Privacy Policy</h1>
            
            <div class="prose prose-lg max-w-none text-gray-700 space-y-6">
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">1. Introduction</h2>
                <p>
                    Afrocentric Visions ("we," "us," "our," or "Company") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you visit our website.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">2. Information We Collect</h2>
                <p>
                    We may collect information about you in a variety of ways. The information we may collect on the Site includes:
                </p>
                <ul class="list-disc pl-6 space-y-2">
                    <li><strong>Personal Data:</strong> Name, email address, phone number, and shipping address when you make a purchase or contact us.</li>
                    <li><strong>Payment Information:</strong> Credit card details and billing information (processed securely through payment providers).</li>
                    <li><strong>Usage Data:</strong> How you interact with our website, including pages visited, time spent, and links clicked.</li>
                    <li><strong>Device Information:</strong> Browser type, IP address, and device type.</li>
                </ul>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">3. How We Use Your Information</h2>
                <p>
                    We use the information we collect for various purposes:
                </p>
                <ul class="list-disc pl-6 space-y-2">
                    <li>To process your orders and send you related information</li>
                    <li>To provide customer service and respond to your inquiries</li>
                    <li>To send promotional emails and marketing materials (with your consent)</li>
                    <li>To improve our website and services</li>
                    <li>To comply with legal obligations</li>
                </ul>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">4. Data Security</h2>
                <p>
                    We implement appropriate technical and organizational measures to protect your personal data against unauthorized access, alteration, disclosure, or destruction. However, no method of transmission over the Internet is 100% secure.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">5. Sharing Your Information</h2>
                <p>
                    We do not sell, trade, or rent your personal information to third parties. We may share information with:
                </p>
                <ul class="list-disc pl-6 space-y-2">
                    <li>Service providers who assist us in operating our website and conducting our business</li>
                    <li>Legal authorities if required by law</li>
                    <li>Business partners with your consent</li>
                </ul>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">6. Your Rights</h2>
                <p>
                    You have the right to:
                </p>
                <ul class="list-disc pl-6 space-y-2">
                    <li>Access your personal data</li>
                    <li>Correct inaccurate data</li>
                    <li>Request deletion of your data</li>
                    <li>Opt-out of marketing communications</li>
                </ul>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">7. Contact Us</h2>
                <p>
                    If you have questions about this Privacy Policy, please contact us at:
                </p>
                <p>
                    Email: <a href="mailto:1stdigitalartistry@gmail.com" class="text-amber-700 hover:text-amber-800">1stdigitalartistry@gmail.com</a>
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">8. Changes to This Policy</h2>
                <p>
                    We may update this Privacy Policy from time to time. We will notify you of any changes by posting the new Privacy Policy on this page.
                </p>

                <p class="text-sm text-gray-500 mt-12">
                    Last updated: <span id="date"></span>
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 pt-12 pb-8">
        <div class="container mx-auto px-4 max-w-7xl text-center">
            <p class="mb-2">
                &copy; <span id="year"></span> Afrocentric Visions. All rights reserved.
            </p>
            <p class="text-sm">
                <a href="index.html" class="text-amber-700 hover:text-amber-600">Back to Home</a> | 
                <a href="privacy.html" class="text-amber-700 hover:text-amber-600">Privacy Policy</a> | 
                <a href="terms.html" class="text-amber-700 hover:text-amber-600">Terms of Service</a>
            </p>
        </div>
    </footer>

    <script>
        document.getElementById('year').textContent = new Date().getFullYear();
        document.getElementById('date').textContent = new Date().toLocaleDateString('en-US', { year: 'numeric', month: 'long', day: 'numeric' });
    </script>
</body>
</html>
```

4. **Save the file** as `privacy.html` in the same folder as your `index.html`

#### **Step 2: Create the Terms of Service File**

1. **Create a new file** in your text editor
2. **Paste this code:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service - Afrocentric Visions">
    <title>Terms of Service - Afrocentric Visions</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-white text-gray-900 font-sans">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="container mx-auto px-4 py-4 max-w-7xl">
            <div class="flex items-center justify-between">
                <div class="flex items-center gap-2">
                    <i class="fas fa-palette text-2xl text-amber-700"></i>
                    <a href="index.html" class="text-2xl font-bold text-gray-900 tracking-tight hover:text-amber-700 transition-smooth">Afrocentric Visions</a>
                </div>
                <a href="index.html" class="text-gray-700 hover:text-amber-700 transition-smooth font-medium">Back to Home</a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-24 bg-white">
        <div class="container mx-auto px-4 max-w-4xl">
            <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8 tracking-tight">Terms of Service</h1>
            
            <div class="prose prose-lg max-w-none text-gray-700 space-y-6">
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">1. Agreement to Terms</h2>
                <p>
                    By accessing and using this website, you accept and agree to be bound by the terms and provision of this agreement. If you do not agree to abide by the above, please do not use this service.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">2. Use License</h2>
                <p>
                    Permission is granted to temporarily download one copy of the materials (information or software) on Afrocentric Visions' website for personal, non-commercial transitory viewing only. This is the grant of a license, not a transfer of title, and under this license you may not:
                </p>
                <ul class="list-disc pl-6 space-y-2">
                    <li>Modify or copy the materials</li>
                    <li>Use the materials for any commercial purpose or for any public display</li>
                    <li>Attempt to decompile or reverse engineer any software contained on the website</li>
                    <li>Remove any copyright or other proprietary notations from the materials</li>
                    <li>Transfer the materials to another person or "mirror" the materials on any other server</li>
                </ul>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">3. Disclaimer</h2>
                <p>
                    The materials on Afrocentric Visions' website are provided on an 'as is' basis. Afrocentric Visions makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties including, without limitation, implied warranties or conditions of merchantability, fitness for a particular purpose, or non-infringement of intellectual property or other violation of rights.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">4. Limitations</h2>
                <p>
                    In no event shall Afrocentric Visions or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of the use or inability to use the materials on Afrocentric Visions' website.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">5. Accuracy of Materials</h2>
                <p>
                    The materials appearing on Afrocentric Visions' website could include technical, typographical, or photographic errors. Afrocentric Visions does not warrant that any of the materials on its website are accurate, complete, or current.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">6. Links</h2>
                <p>
                    Afrocentric Visions has not reviewed all of the sites linked to its website and is not responsible for the contents of any such linked site. The inclusion of any link does not imply endorsement by Afrocentric Visions of the site. Use of any such linked website is at the user's own risk.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">7. Modifications</h2>
                <p>
                    Afrocentric Visions may revise these terms of service for its website at any time without notice. By using this website, you are agreeing to be bound by the then current version of these terms of service.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">8. Governing Law</h2>
                <p>
                    These terms and conditions are governed by and construed in accordance with the laws of the jurisdiction in which Afrocentric Visions operates, and you irrevocably submit to the exclusive jurisdiction of the courts in that location.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">9. Purchase and Refund Policy</h2>
                <p>
                    <strong>Satisfaction Guarantee:</strong> We offer a 100% satisfaction guarantee on all purchases. If you are not satisfied with your purchase, you may request a refund within 30 days of purchase.
                </p>
                <ul class="list-disc pl-6 space-y-2">
                    <li><strong>Digital Products:</strong> Full refund available within 30 days of purchase</li>
                    <li><strong>Framed Artwork:</strong> Returns accepted within 30 days if damaged or not as described</li>
                    <li><strong>Refund Process:</strong> Contact us at 1stdigitalartistry@gmail.com to initiate a return</li>
                </ul>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">10. Intellectual Property Rights</h2>
                <p>
                    All content on this website, including artwork, images, text, and designs, is the property of Afrocentric Visions or its content suppliers and is protected by international copyright laws. You may not reproduce, distribute, or transmit any content without written permission.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">11. Contact Us</h2>
                <p>
                    If you have any questions about these Terms of Service, please contact us at:
                </p>
                <p>
                    Email: <a href="mailto:1stdigitalartistry@gmail.com" class="text-amber-700 hover:text-amber-800">1stdigitalartistry@gmail.com</a>
                </p>

                <p class="text-sm text-gray-500 mt-12">
                    Last updated: <span id="date"></span>
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 pt-12 pb-8">
        <div class="container mx-auto px-4 max-w-7xl text-center">
            <p class="mb-2">
                &copy; <span id="year"></span> Afrocentric Visions. All rights reserved.
            </p>
            <p class="text-sm">
                <a href="index.html" class="text-amber-700 hover:text-amber-600">Back to Home</a> | 
                <a href="privacy.html" class="text-amber-700 hover:text-amber-600">Privacy Policy</a> | 
                <a href="terms.html" class="text-amber-700 hover:text-amber-600">Terms of Service</a>
            </p>
        </div>
    </footer>

    <script>
        document.getElementById('year').textContent = new Date().getFullYear();
        document.getElementById('date').textContent = new Date().toLocaleDateString('en-US', { year: 'numeric', month: 'long', day: 'numeric' });
    </script>
</body>
</html>
```

3. **Save the file** as `terms.html` in the same folder as your `index.html`

#### **Step 3: Verify Your Files Are Saved**

Your project folder should now look like this:

```
Your Project Folder/
├── index.html
├── privacy.html
└── terms.html
```

### Customizing the Privacy and Terms Pages

#### **Update Company Name**

In both `privacy.html` and `terms.html`, find and replace:
- `Afrocentric Visions` → Your company name
- `1stdigitalartistry@gmail.com` → Your email address

#### **Update Specific Sections**

**In privacy.html:**
- Change section 2 (Information We Collect) to match what you actually collect
- Update section 3 (How We Use Your Information) with your actual practices
- Modify section 7 (Contact Us) with your contact details

**In terms.html:**
- Update section 8 (Governing Law) with your jurisdiction
- Modify section 9 (Purchase and Refund Policy) to match your actual policy
- Update section 11 (Contact Us) with your information

### Method 2: Use a Terms Generator (Faster Alternative)

If you want to generate professional legal documents quickly:

1. **Visit** [Termly.io](https://termly.io) or [TermsFeed.com](https://www.termsfeed.com)
2. **Answer their questions** about your business
3. **Download the generated documents**
4. **Save as** `privacy.html` and `terms.html`
5. **Copy the content** into the HTML templates provided above

### Testing Your Links

**After creating the privacy and terms pages:**

1. **Save all three files** (`index.html`, `privacy.html`, `terms.html`) in the same folder
2. **Open `index.html` in your browser**
3. **Click the "Privacy Policy" link** in the footer - it should open `privacy.html`
4. **Click the "Terms of Service" link** - it should open `terms.html`
5. **On the policy pages, click "Back to Home"** - it should return to `index.html`

### Troubleshooting: Links Not Working

**Problem:** Clicking "Privacy Policy" does nothing

**Solutions:**
1. Make sure `privacy.html` is saved in the same folder as `index.html`
2. Check the filename is exactly `privacy.html` (lowercase, no spaces)
3. Verify the link in `index.html` says `href="privacy.html"`
4. Refresh your browser (Ctrl+R or Cmd+R)

**Problem:** "Page not found" error

**Solutions:**
1. Check the file path in the `href` attribute
2. Make sure the filename matches exactly (case-sensitive)
3. Verify all files are in the same directory
4. Try using the full path: `href="./privacy.html"`

---

## Troubleshooting Guide

### Common Issues and Solutions

#### **1. Styles Not Showing (Page Looks Broken)**

**Problem:** The page looks plain without colors or proper layout

**Causes:**
- Tailwind CSS CDN not loading
- Internet connection issue
- Browser cache problem

**Solutions:**
```html
<!-- Check this line exists in your <head> section -->
<script src="https://cdn.tailwindcss.com"></script>
```

If it's there:
1. **Clear browser cache** (Ctrl+Shift+Delete)
2. **Hard refresh the page** (Ctrl+Shift+R or Cmd+Shift+R)
3. **Check your internet connection**
4. **Try a different browser**

#### **2. Images Not Displaying**

**Problem:** You see broken image icons instead of pictures

**Causes:**
- Image URL is broken
- External image service is down
- Wrong file path

**Solution:**
Replace the image URL with a working one:

```html
<!-- Current broken image -->
<img src="https://images.unsplash.com/photo-1504093376055-b3094b674dcb?w=1600&h=900&fit=crop&q=80" alt="Art">

<!-- Replace with your own image -->
<img src="your-image.jpg" alt="Your art description">
```

#### **3. Mobile Menu Not Working**

**Problem:** The hamburger menu doesn't open on mobile devices

**Causes:**
- JavaScript not loading
- Mobile menu button not clickable
- CSS display issue

**Solution:**
1. **Check JavaScript is enabled** in your browser
2. **Verify this code exists** at the bottom of your HTML:
```javascript
<script>
    const mobileMenuButton = document.querySelector('.mobile-menu-button');
    const mobileMenu = document.querySelector('.mobile-menu');

    mobileMenuButton.addEventListener('click', function() {
        mobileMenu.classList.toggle('show');
    });
</script>
```

3. **Test on a real mobile device** or use browser DevTools (F12)

#### **4. Links Opening in Wrong Place**

**Problem:** Clicking a link opens the wrong page or doesn't navigate

**Causes:**
- Wrong `href` value
- Missing `#` for internal links
- File doesn't exist

**Solution:**
```html
<!-- Internal link (same page) - must start with # -->
<a href="#features">Go to Features</a>

<!-- External link - must have full URL -->
<a href="https://example.com">Visit Example</a>

<!-- Email link -->
<a href="mailto:your@email.com">Email Us</a>
```

#### **5. Form Not Submitting**

**Problem:** Clicking "Send Message" does nothing

**Causes:**
- Form action not set
- Form validation failing
- JavaScript error

**Solution:**
```html
<!-- Add action attribute to form -->
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
    <!-- form fields -->
</form>
```

Get a free form ID from [Formspree.io](https://formspree.io)

#### **6. Responsive Design Broken**

**Problem:** Page looks wrong on tablets or phones

**Causes:**
- Viewport meta tag missing
- Tailwind responsive classes removed
- Browser zoom issue

**Solution:**
Verify this line exists in your `<head>`:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

#### **7. Smooth Scrolling Not Working**

**Problem:** Clicking menu links doesn't smoothly scroll to sections

**Causes:**
- CSS scroll-behavior disabled
- JavaScript scroll function broken
- Section IDs don't match

**Solution:**
1. **Verify this CSS exists:**
```css
* {
    scroll-behavior: smooth;
}
```

2. **Check section IDs match links:**
```html
<!-- Link points to #features -->
<a href="#features">Features</a>

<!-- Section must have matching ID -->
<section id="features">...</section>
```

#### **8. Colors Not Changing**

**Problem:** Changed a color class but nothing happened

**Causes:**
- Tailwind class name misspelled
- Browser cache not cleared
- Conflicting CSS

**Solution:**
1. **Check the class name** is spelled correctly
2. **Clear browser cache** (Ctrl+Shift+Delete)
3. **Hard refresh** (Ctrl+Shift+R)
4. **Verify the class is a valid Tailwind class**

```html
<!-- Valid -->
<div class="bg-amber-700">Box</div>

<!-- Invalid (won't work) -->
<div class="bg-amber-750">Box</div>  <!-- 750 doesn't exist -->
```

#### **9. Text Too Small or Too Large**

**Problem:** Heading or body text size is wrong

**Solution:**
```html
<!-- Text size classes -->
<p class="text-sm">Small text</p>
<p class="text-base">Normal text</p>
<p class="text-lg">Large text</p>
<h1 class="text-4xl">Heading</h1>
<h1 class="text-6xl">Larger heading</h1>
```

#### **10. Spacing Issues**

**Problem:** Too much or too little space between elements

**Solution:**
```html
<!-- Padding (inside) -->
<div class="p-4">More padding inside</div>
<div class="p-8">Even more padding</div>

<!-- Margin (outside) -->
<div class="mb-4">Space below</div>
<div class="mt-8">More space above</div>

<!-- Gap (between items) -->
<div class="flex gap-4">Item 1</div>
<div class="flex gap-8">Item 1</div>
```

### Getting Help

**If you're stuck:**

1. **Check the browser console** for errors (F12 → Console tab)
2. **Compare your code** to the original provided HTML
3. **Search for the error message** online
4. **Try reverting recent changes** to find what broke
5. **Validate your HTML** at [W3C Validator](https://validator.w3.org)

---

## Best Practices

### 1. **Always Make Backups**

Before making major changes:
1. **Save a copy** of your HTML file
2. **Name it** `index-backup.html`
3. **Keep it** in the same folder
4. **If something breaks**, you can restore from backup

### 2. **Make One Change at a Time**

**Good workflow:**
1. Make one small change
2. Save the file
3. Refresh browser to test
4. If it works, keep the change
5. If it breaks, undo the change
6. Move to next change

### 3. **Use Meaningful Section IDs**

```html
<!-- Good - clear and descriptive -->
<section id="features">...</section>
<section id="testimonials">...</section>

<!-- Bad - unclear -->
<section id="section1">...</section>
<section id="content">...</section>
```

### 4. **Keep Consistent Styling**

Use the same colors, spacing, and fonts throughout:
```html
<!-- Consistent -->
<h2 class="text-4xl md:text-5xl font-bold text-gray-900">Title</h2>
<p class="text-xl text-gray-600">Description</p>

<!-- Inconsistent -->
<h2 class="text-3xl font-normal text-blue-900">Title</h2>
<p class="text-base text-gray-500">Description</p>
```

### 5. **Test on Multiple Devices**

Test your page on:
- Desktop browser
- Tablet (iPad or similar)
- Mobile phone
- Different browsers (Chrome, Firefox, Safari)

### 6. **Optimize Images**

- Keep images under 500KB
- Use web-friendly formats (JPG, PNG, WebP)
- Use descriptive alt text: `alt="Customer smiling in front of art"`

### 7. **Update Content Regularly**

- Refresh testimonials quarterly
- Update featured products seasonally
- Keep contact information current
- Review and update policies annually

### 8. **Use Descriptive Link Text**

```html
<!-- Good - clear what the link is -->
<a href="#features">Learn about our features</a>

<!-- Bad - unclear -->
<a href="#features">Click here</a>
```

### 9. **Keep File Organization**

```
project-folder/
├── index.html
├── privacy.html
├── terms.html
├── images/
│   ├── logo.png
│   └── hero.jpg
└── css/
    └── custom-styles.css (if you add custom CSS)
```

### 10. **Document Your Changes**

Add comments to remember why you made changes:

```html
<!-- Changed hero headline color from white to light gray on 2024-01-15 -->
<h1 class="text-white">Headline</h1>

<!-- Added new testimonial from customer review - 2024-01-20 -->
<div class="testimonial">...</div>
```

---

## Quick Reference: Common Tasks

### Change Primary Color (Amber → Blue)

Find and replace all instances:
- `text-amber-700` → `text-blue-700`
- `bg-amber-700` → `bg-blue-700`
- `hover:bg-amber-800` → `hover:bg-blue-800`
- `hover:text-amber-700` → `hover:text-blue-700`

### Add a New Feature Card

Copy this template and add it to the Features section:

```html
<div class="bg-white border border-gray-200 rounded-xl p-8 transition-smooth hover-lift hover:shadow-xl hover:border-amber-700">
    <div class="bg-amber-100 w-16 h-16 rounded-lg flex items-center justify-center mb-6">
        <i class="fas fa-star text-amber-700 text-2xl"></i>
    </div>
    <h3 class="text-2xl font-bold text-gray-900 mb-3">Your Feature Title</h3>
    <p class="text-gray-600 leading-relaxed mb-4">
        Your feature description goes here.
    </p>
    <ul class="space-y-2 text-sm text-gray-600">
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-amber-700"></i>
            Feature benefit 1
        </li>
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-amber-700"></i>
            Feature benefit 2
        </li>
    </ul>
</div>
```

### Add a New Testimonial

Copy this template and add it to the Testimonials section:

```html
<div class="bg-white rounded-xl p-8 shadow-md transition-smooth hover-lift hover:shadow-lg border border-gray-200">
    <div class="flex items-center gap-1 mb-4">
        <i class="fas fa-star text-amber-700"></i>
        <i class="fas fa-star text-amber-700"></i>
        <i class="fas fa-star text-amber-700"></i>
        <i class="fas fa-star text-amber-700"></i>
        <i class="fas fa-star text-amber-700"></i>
    </div>
    <p class="text-gray-700 leading-relaxed mb-6 text-lg">
        "Your testimonial text goes here."
    </p>
    <div class="flex items-center gap-4">
        <div class="w-12 h-12 bg-gradient-to-br from-amber-400 to-orange-500 rounded-full flex items-center justify-center text-white font-bold">
            AB
        </div>
        <div>
            <p class="font-bold text-gray-900">Customer Name</p>
            <p class="text-sm text-gray-600">Job Title, City</p>
        </div>
    </div>
</div>
```

### Add a New FAQ Item

Copy this template and add it to the FAQ section:

```html
<div class="faq-item">
    <button class="faq-toggle w-full text-left py-6 px-6 bg-gray-50 hover:bg-gray-100 rounded-lg transition-smooth flex items-center justify-between font-semibold text-lg text-gray-900">
        <span>Your question here?</span>
        <i class="fas fa-chevron-down text-amber-700"></i>
    </button>
    <div class="faq-answer px-6 pb-6">
        <p class="text-gray-700 leading-relaxed">
            Your answer goes here.
        </p>
    </div>
</div>
```

---

## Final Checklist

Before launching your website, verify:

- [ ] All text content is updated
- [ ] Brand name and logo are correct
- [ ] Contact email is accurate
- [ ] All links work correctly
- [ ] Images display properly
- [ ] Mobile menu works on phones
- [ ] Form submissions work
- [ ] Privacy policy page is accessible
- [ ] Terms of service page is accessible
- [ ] Social media links are correct
- [ ] Page looks good on mobile and desktop
- [ ] No broken images or missing icons
- [ ] Footer information is current
- [ ] SEO meta tags are updated
- [ ] Smooth scrolling works

---

## Additional Resources

### Learning Resources
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [HTML Beginner Guide](https://www.w3schools.com/html/)
- [Font Awesome Icons](https://fontawesome.com/icons)
- [MDN Web Docs](https://developer.mozilla.org/)

### Tools
- [HTML Validator](https://validator.w3.org)
- [Color Picker](https://colorpicker.com)
- [Responsive Design Tester](https://responsivedesignchecker.com)
- [Formspree](https://formspree.io) - Form submissions

### Hosting Options
- [Netlify](https://netlify.com) - Free hosting
- [Vercel](https://vercel.com) - Free hosting
- [GitHub Pages](https://pages.github.com) - Free hosting
- [Bluehost](https://bluehost.com) - Paid hosting

---

## Support

For questions or issues with this landing page:

**Email:** 1stdigitalartistry@gmail.com

**Before contacting support, please:**
1. Check this guide for solutions
2. Clear your browser cache
3. Try a different browser
4. Verify all files are in the same folder
5. Check the browser console for errors (F12)

---

**Last Updated:** January 2024  
**Version:** 1.0  
**Compatibility:** All modern browsers (Chrome, Firefox, Safari, Edge)

This comprehensive guide should help you maintain and customize your Afrocentric Visions landing page with confidence, even if you're new to web development!