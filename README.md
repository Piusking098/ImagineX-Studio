# ImagineX Studio — Creative Portfolio Website
**Founder & Lead Creative Director:** Pius Christopher  
**Brand Identity:** ImagineX Studio  

---

## Overview
A modern, dark glassmorphic, high-converting portfolio website built for **ImagineX Studio (Pius Christopher)**. It showcases 78 curated creative design projects spanning swipeable carousels, commercial ad campaigns, FinTech social suites, church sermon series, gourmet restaurant menus, food packaging, and minimalist brand identity vector logos.

---

## Key Features & Capabilities

1. **78 Curated Projects Showcase**:
   - **NowNow (19 items)**: Customer review carousel deck, recruitment flyers, holiday features, and 16 commercial social media retainers.
   - **JBUIT Technologies (9 items)**: "Get a Business Website" 7-slide sales carousel, AI course masterclass flyers, full-stack web flyers, mobile app flyers, and curriculum guides.
   - **Holyspirit Hub Ministries (15 items)**: 6-slide sequential sermon notes carousel, worship night posters, miracle service graphics, and daily devotional cards.
   - **Child of Wealth Initiative (COWI) (3 items)**: 7-slide TEL Bootcamp Cohort 1 carousel, youth leadership webinar flyer, and World Food Day global nutrition advocacy poster.
   - **Creaverse Studio (2 items)**: "Speed Up Your Brand" creative agency campaign and "Beyond The Icon" holistic brand identity social post.
   - **Abikè Olòròrò (2 items)**: 3D commercial vegetable oil product ad poster and "Every Meal Has A Beginning" culinary campaign flyer.
   - **Smoothiezee (1 item)**: Gourmet sandwich box packaging design and fresh bottled juice morning breakfast combo visual.
   - **Ask Abike (1 item)**: "When Favoritism Replaces Fairness" executive thought-leadership quote card.
   - **Studio Originals (26 items)**: Church & worship posters, gourmet restaurant menu layouts, precision vector logomarks, new month greetings, and creative social ads.

2. **Dual Filter & Real-Time Keyword Search**:
   - Filter by **Client Brand** (All Projects, NowNow, JBUIT, Holyspirit Hub, COWI, Creaverse, Abikè Olòròrò, Smoothiezee, Ask Abike, Studio Originals).
   - Filter by **Category Discipline** (Swipeable Carousels, Posters & Flyers, Social Media, Church & Events, Restaurant & Menus, Logos & Branding, New Month & Seasonal).
   - Instant search bar with live filtering by project title, description, brand, or hashtags.
   - Progressive "Load More" pagination with native lazy-loading for lightning-fast performance.

3. **Interactive Viewers & Modals**:
   - **Multi-Slide Carousel Deck Modal**: Swipe gestures on mobile, Left/Right arrow keys, auto-slideshow toggle, slide counter (`Slide X of Y`), and active thumbnail navigation strip.
   - **High-Resolution Lightbox**: Detailed view of single posters, packaging, menus, and logomarks with quick "Inquire Similar Style" action.
   - **4 Flagship Case Studies**: Slide-out drawer featuring client brief, creative strategy, quantified impact metrics, deliverables checklist, and clickable asset gallery.
   - **Dual-Channel Contact Engine**: Direct WhatsApp messaging with pre-filled text (+234 814 077 7495) or email routing (imaginex82@gmail.com).
   - **One-Click "Copy Email"**: Instant visual confirmation tooltip.

4. **Strategic Conversion Sections**:
   - **4-Step Creative Process**: Discovery -> Moodboard -> High-Fidelity Crafting -> Delivery.
   - **Service Retainer Packages**: Design Sprint (24-48h), Monthly Social Retainer (15-25 assets), and Full Brand Identity System.
   - **Client Testimonials & Social Proof**: 6 verified client reviews from Director Biggs, Vivi Couture, Fat man Kitchen, Giwu Treats, Shavionb, and Tiana Clothings.
   - **Interactive FAQ Accordion**: Clear answers to client turnaround, source file formats, revisions, and payment options.

---

## File Structure

```
Portfolio website/
│
├── index.html              # Main website markup, glassmorphism CSS, and interactive JS engine
├── portfolio-data.js       # Complete 78-item dataset with titles, tags, covers, and carousel slides
├── README.md               # Project documentation and deployment guide
└── assets/                 # High-resolution design assets organized by client and category
    ├── brands/
    │   ├── Abike Olororo/  # 3D product renders and commercial culinary campaign flyers
    │   ├── Ask_Abike/      # Executive thought-leadership cards
    │   ├── cowi/           # Bootcamp carousels, webinar flyers, World Food Day poster
    │   ├── Creaverse/      # Agency brand acceleration campaigns and identity visuals
    │   ├── holyspirit-hub/ # Sermon carousels, worship posters, social posts
    │   ├── jbuit/          # Website carousels, tech flyers, new month greetings
    │   ├── nownow/         # Review carousels, campaign flyers, 16 social posts
    │   └── Smoothiezee/    # Fast-casual sandwich box packaging and juice branding
    ├── church-flyers/      # Original worship & prayer gathering posters
    ├── restaurant-menu-design/ # Gourmet food & beverage menu layouts
    ├── logo-design/        # Precision vector brandmarks and logotypes
    ├── social-post-design/ # High-impact commercial social media creatives
    ├── new-month-design/   # Seasonal and new month celebration visuals
    ├── me/                 # Pius Christopher founder headshots and logo files
    ├── logo.png            # ImagineX Studio primary brand logo
    └── favicon.ico         # Studio browser favicon
```

---

## How to Add New Projects

To add a new project to your portfolio, simply open `portfolio-data.js` and add an object to the `portfolioItems` array:

### For Single Image (Flyer, Logo, Menu, Social Post):
```javascript
{
    id: "my-new-project",
    brand: "Brand Name", // e.g. "NowNow", "Studio Originals", or your new client
    category: "Posters & Flyers", // "Carousels", "Social Media", "Church & Events", "Restaurant & Menus", "Logos & Branding", "New Month"
    tags: ["Flyer", "Commercial", "Event"],
    title: "Project Title Here",
    badge: "Event Flyer",
    isCarousel: false,
    cover: "assets/path/to/your/image.png",
    desc: "Brief description of the design and strategic impact."
}
```

### For Multi-Slide Carousel Deck:
```javascript
{
    id: "my-new-carousel",
    brand: "Brand Name",
    category: "Carousels",
    tags: ["Carousel", "Educational", "Social"],
    title: "Carousel Title Here",
    badge: "5-Slide Deck",
    isCarousel: true,
    cover: "assets/path/to/slide-1.png",
    slides: [
        "assets/path/to/slide-1.png",
        "assets/path/to/slide-2.png",
        "assets/path/to/slide-3.png",
        "assets/path/to/slide-4.png",
        "assets/path/to/slide-5.png"
    ],
    desc: "Multi-slide educational carousel designed for high saves and shares."
}
```

---

## Free Hosting & Deployment

Your website is 100% static, fast, and requires zero build tools. You can deploy it for free within 2 minutes:

### Option A: Vercel (Recommended)
1. Push your folder to a GitHub repository or install Vercel CLI (`npm i -g vercel`).
2. Run `vercel` in this folder, or import the GitHub repo on [vercel.com](https://vercel.com).
3. Instant global SSL, CDN, and ultra-fast loading.

### Option B: Netlify
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop).
2. Drag and drop this `Portfolio website` folder.
3. Your website is live immediately with an HTTPS link and custom domain support.

### Option C: GitHub Pages
1. Push the files to a repository named `<your-username>.github.io`.
2. Go to **Settings** > **Pages** > Select **main branch** as source.
3. Your portfolio will be live at `https://<your-username>.github.io`.

---

## Studio Contact Information
- **WhatsApp:** [+234 814 077 7495](https://wa.me/2348140777495)
- **Email:** [imaginex82@gmail.com](mailto:imaginex82@gmail.com)
- **Founder:** Pius Christopher

