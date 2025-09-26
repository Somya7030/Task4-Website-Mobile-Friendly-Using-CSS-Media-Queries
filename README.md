📝 Project Overview
This project demonstrates how to convert a desktop-only webpage into a mobile-friendly responsive layout using CSS media queries.
The webpage adjusts its layout and styles based on the device’s screen size to ensure a better user experience on both desktop and mobile devices.

🎯 Objectives
Grasp media queries and their use.
Understand mobile-first design.
Create flexible layouts with CSS.
Make images and navigation responsive.

🛠 Tools & Technologies
HTML5
CSS3
VS Code
Chrome DevTools (for testing responsiveness)

🚀 Features
✔ Responsive 2-column layout (desktop) → stacks vertically on mobile.
✔ Navigation menu switches from horizontal to vertical on small screens.
✔ Images scale properly within containers (max-width: 100%).
✔ Font sizes & spacing adjust for readability on smaller devices.
✔ Uses standard breakpoint: 768px for tablets & phones.

📂 File Structure
Responsive-Blog/
│
├── index.html      # Main webpage
└── README.md       # Project documentation

📐 Code Snippets

1️⃣ Viewport Meta Tag (ensures mobile scaling):

<meta name="viewport" content="width=device-width, initial-scale=1.0">


2️⃣ Responsive Images (scales within container):

img {
  max-width: 100%;
  height: auto;
}


3️⃣ Media Query for Mobile (≤ 768px):

@media (max-width: 768px) {
  .container {
    flex-direction: column; /* stack sidebar + content */
  }

  nav ul {
    flex-direction: column; /* vertical menu */
    align-items: center;
    gap: 10px;
  }

  body {
    font-size: 14px; /* smaller text on mobile */
  }
}


📱 Testing Responsiveness

Open the project in Google Chrome.
Right-click → Inspect → Toggle Device Toolbar (Ctrl+Shift+M).
Test on different devices (mobile, tablet, desktop).
Ensure no horizontal scrolling and layout adapts smoothly.

✅ Deliverables

index.html → Updated webpage with responsive CSS.
README.md → Documentation (this file).
