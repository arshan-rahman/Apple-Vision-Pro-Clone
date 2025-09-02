# 📖 Detailed Documentation: Apple Vision Pro Clone Website

This document provides an in-depth look at the structure, design, and animations used in the Apple Vision Pro clone website.

---

## 1. Overview
The project recreates Apple’s **Vision Pro showcase** with:  
- Scroll-driven interactions  
- Canvas animations for 3D rotation  
- Alternating fullscreen videos & static sections  

It’s fully front-end, built with **HTML, CSS, and JavaScript**.


---

## 2. Page-by-Page Breakdown

### 🔹 Landing Page (`#page`)
- **Content:**  
  - Intro video (`intro1.mp4`)  
  - Navigation bar with *Vision Pro* + *Notify Me* button  
  - Bottom logo with introduction text  
- **Animations:**  
  - Nav fades in (GSAP stagger)  
  - Video starts on scroll  
  - Section is **pinned**  

---

### 🔹 Page 1 (`#page1`)
- **Video:** `second.mp4` looping  
- **Headline:** *“Welcome to the era of spatial computing”*  
- **Animation:** Headline scrolls upward and fades  

---

### 🔹 Page 2 (`#page2`)
- **Video:** `third1.mp4`  
- **Headline:** Blending digital & physical spaces  
- **Animation:** Same scroll-up effect as Page 1  

---

### 🔹 Page 3 (`#page3`)
- **Content:** Apple logo, Vision Pro image, CTA button  
- **Design:** Dark background for dramatic product reveal  

---

### 🔹 Page 4 (`#page4`)
- **Video:** `page4keke.mp4`  
- **Content:** Apps headline → *“Free your desktop. And your apps will follow.”*  
- **Animation:** Center text scrolls upward  

---

### 🔹 Page 5 (`#page5`)
- **Layout:**  
  - Left: Headline  
  - Right: Paragraph text + CTA button  
- **Animation:**  
  - Left text slides in from left  
  - Right text + button fade in sequentially  

---

### 🔹 Page 6 (`#page6`)
- **Section:** *“Designed by Apple.”*  
- **Details:** Hardware materials + light seal description  
- **Animation:** Text elements fade in with scroll  

---

### 🔹 Page 7 (`#page7`)
- **Canvas Animation:**  
  - Renders **360° Vision Pro rotation** (frames 0000–0199) from Apple CDN  
  - Scroll controls the sequence  
- **Interaction:** Section pinned for extended scroll effect  

---

### 🔹 Pages 8–13
- **Individual feature highlights:**  
  - Page 8 → Enclosure  
  - Page 9 → Light Seal  
  - Page 10 → Head Band  
  - Page 11 → Power  
  - Page 12 → Sound  
  - Page 13 → EyeSight  
- **Layout:** Alternating left/right aligned text  

---

### 🔹 Page 14 (`#page14`)
- Split layout: Two large side-by-side product images  

---

### 🔹 Page 15 (`#page15`)
- Fullscreen video section (`center.mp4`)  

---

### 🔹 Page 16 (`#page16`)
- **Content:** Detailed description of laminated glass & light seal  
- **Media:** Supporting vertical image (`vertical.jpg`)  
- **CTA:** *“Learn more about design”* button  

---

### 🔹 Page 18 (`#page18`)
- **Canvas Animation:**  
  - Local Vision Pro render sequence (`Vision00001.png` → …)  

---

### 🔹 Page 19 (`#page19`)
- **Text Highlight:**  
  - *“More pixels than a 4K TV. For each eye.”*  
  - Subtext: Micro-OLED display + lenses  

---

### 🔹 Page 20 (`#page20`)
- **Video:** Spatial Audio demo  
- **Text Box:** Positioned bottom-right, describes sound features  

---

### 🔹 Pages 21–23
- Page 21 → Eye Tracking images (`tron`/`troff`)  
- Page 22 → Sensor visualization (`snron`/`snroff`)  
- Page 23 → Static product image (chips & sensors)  

---

## 3. Styling (style.css)
- Minimal Apple-style design  
- Alternating **dark/light backgrounds**  
- Fullscreen videos with centered text overlays  
- Rounded CTA buttons with orange highlights  
- Flexbox layouts for split sections  

---

## 4. Scripts (script.js)
- **Locomotive Scroll** → Smooth scrolling  
- **GSAP + ScrollTrigger** →  
  - Pinned sections  
  - Text fades & movement  
  - Sequential animations  
- **Canvas Animations** →  
  - Frame-by-frame image loading  
  - Scroll-driven 3D effect  

---

## 5. Notes
- Heavy assets (videos & images) → preload recommended  
- Canvas animations may lag on low-end devices  
- Purely **front-end showcase** (no backend functionality)  

---

## 6. Credits
- Apple Inc. (inspiration & media assets)  
- [GSAP](https://greensock.com/gsap/)  
- [Locomotive Scroll](https://github.com/locomotivemtl/locomotive-scroll)  

