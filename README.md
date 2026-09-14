# DP PDF COMPARE

> **Zero-Knowledge Enterprise Visual PDF Comparator**  
> Compare multiple PDF documents visually right inside your web browser. 100% private, air-gapped, and local.

---

## 🔒 Confidentiality & Security Architecture

`DP PDF COMPARE` was built for environments where uploading sensitive documents, architectural blueprints, contracts, or engineering drawings to third-party cloud services poses a compliance or security risk.

* **Client-Side Execution:** Documents are decoded locally in your browser’s V8 JavaScript engine via WebAssembly/Canvas APIs.
* **Zero Network Transfers:** No API endpoints, external databases, or remote servers are contacted during file processing.
* **Volatile Memory Storage:** Canvas data and page vectors exist strictly within temporary browser RAM.
* **Offline Capable:** The entire application works seamlessly while completely disconnected from the internet or Wi-Fi.

---

## ✨ Features

* 📄 **Multi-PDF Comparison:** Compare up to 5 PDF layers simultaneously.
* 🎨 **Custom Color Pickers:** Assign distinct visual highlight signatures for every loaded layer.
* 👁️ **Dual Display Modes:**
  * **Full Visual Overlay Mode:** Displays all layers stacked, showing base elements in dark slate and differences in custom colors.
  * **Differences Only Mode:** Filters out all matching background elements to reveal only modified/added geometry and text.
* 🧹 **Direct Cache Purging:** Clean your browser's active RAM canvas memory with a single click.
* 📱 **Modern Glassmorphic UI:** Built with Tailwind CSS and Lucide icons for an enterprise-ready dark interface.

---

## 🚀 Getting Started

### Option A: Run Locally (No Installation Required)
1. Download or clone this repository to your computer.
2. Double-click `index.html`.
3. The app will launch instantly in your browser of choice (Chrome, Edge, Firefox, Safari).

### Option B: Deploy to Static Hosting
Since this is a client-side static application, you can host it for free on any static web platform:
* **GitHub Pages**
* **Vercel**
* **Netlify**
* **AWS S3 / Cloudflare Pages**

*(Note: Hosting the static HTML file online does not compromise security—all PDF comparisons remain local to the visiting user's device.)*

---

## 📖 How to Use

1. **Select Number of Layers:** Choose how many PDF files you wish to compare (2 to 5) from the dropdown menu.
2. **Assign Layer Colors:** Use the color pickers to assign a distinct accent color for each PDF file.
3. **Upload Files:** Click **Choose File** for each layer to load your target PDF documents.
4. **Choose Display Mode:** Select either **Full Visual Overlay Mode** or **Differences Only Mode**.
5. **Render:** Click **Render High-Precision Comparison** to display the visual matrix.
6. **Purge Cache:** Click **Purge Cache** in the top navigation bar at any time to clear stored memory.

---

## 🛠️ Tech Stack

* **Structure & UI:** HTML5, Tailwind CSS (v3 CDN), Lucide Icons
* **Rendering Engine:** PDF.js (v2.16) by Mozilla
* **Graphics Engine:** HTML5 Canvas API (Pixel matrix difference blending)

---

## 📄 License

Distributed under the MIT License. Feel free to use, modify, and distribute for private or commercial use.
