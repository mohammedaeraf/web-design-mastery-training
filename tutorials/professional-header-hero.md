# 🌐 **Guidance: How to Build a Professional Header + Hero Section**

A strong header + hero section sets the tone of an entire website. Teach students to follow these principles:

## ✅ **1. Keep the Header Clean & Minimal**

* Logo on the left
* Navigation links on the right
* Avoid too many menu items (5–6 max)
* Use proper spacing & alignment
* Use contrasting background (white/dark)
* Use Bootstrap’s `.navbar` for mobile-friendly design

## ✅ **2. Ensure Mobile Responsiveness**

A professional header ALWAYS has:

* Collapsible mobile menu
* Clear nav items
* Clickable logo
* Hamburger icon on mobile

Bootstrap handles 90% of this automatically.

## ✅ **3. Hero Section Must Be High-Impact**

A hero section must include:

* A big heading
* A simple sub-heading
* One or two call-to-action buttons (CTA)
* A relevant image or background
* Clean spacing + balanced layout

## 🎨 **Visual Design Tips**

* Use white space generously
* Keep font sizes bold & readable
* Make CTAs the highlight (e.g., "Get Started")
* Keep alignment consistent
* Don’t mix too many colors

---

# 🧑‍💻 **Sample Code: Professional Header Using Bootstrap (Responsive)**

> This is clean, modern, and perfect for students to learn.

```html
<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- HEADER START -->
<nav class="navbar navbar-expand-lg navbar-light bg-white shadow-sm py-3">
  <div class="container">
    <a class="navbar-brand fw-bold fs-4" href="#">FLA Academy</a>

    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
      <ul class="navbar-nav gap-3">
        <li class="nav-item">
          <a class="nav-link active fw-semibold" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link fw-semibold" href="#">Courses</a>
        </li>
        <li class="nav-item">
          <a class="nav-link fw-semibold" href="#">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link fw-semibold" href="#">Contact</a>
        </li>
        <li class="nav-item">
          <a class="btn btn-primary px-4" href="#">Enroll Now</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
<!-- HEADER END -->
```

---

# 🖼️ **Sample Hero Section (Professional + Bootstrap)**

```html
<section class="py-5 bg-light">
  <div class="container py-5">
    <div class="row align-items-center">
      
      <div class="col-lg-6">
        <h1 class="display-4 fw-bold mb-3">
          Build Modern, Responsive Websites with Confidence
        </h1>
        <p class="lead mb-4">
          Join our Web Design Mastery program and learn real-world skills through hands-on projects and industry-level layouts.
        </p>
        <a href="#" class="btn btn-primary btn-lg px-4 me-3">Get Started</a>
        <a href="#" class="btn btn-outline-dark btn-lg px-4">View Syllabus</a>
      </div>

      <div class="col-lg-6 text-center mt-4 mt-lg-0">
        <img src="https://via.placeholder.com/500x350" class="img-fluid rounded shadow" alt="Hero Image">
      </div>

    </div>
  </div>
</section>
```

---

# ✔ What Students Learn From This Example

* How to build a responsive header using Bootstrap
* How to use `navbar`, `container`, `collapse`, `navbar-toggler`
* How to create a modern hero layout
* How to align elements using Bootstrap grid
* How to use CTAs effectively
* Clean, structured, and industry-standard HTML
