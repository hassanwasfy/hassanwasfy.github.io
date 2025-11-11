<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Hassan Wasfy | Android Engineer</title>
    <meta
      name="description"
      content="Hassan Wasfy is an Android engineer crafting mobile apps, open-source libraries, and reliable product experiences."
    />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap"
      rel="stylesheet"
    />
    <style>
      :root {
        --surface: rgba(15, 23, 42, 0.7);
        --surface-strong: rgba(15, 23, 42, 0.9);
        --accent: #38bdf8;
        --text-primary: #f8fafc;
        --text-secondary: #cbd5f5;
        --muted: rgba(148, 163, 184, 0.6);
        --nav-width: 270px;
        --gap: 2.5rem;
      }

      * {
        box-sizing: border-box;
      }

      html {
        scroll-behavior: smooth;
      }

      body {
        margin: 0;
        font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI",
          sans-serif;
        color: var(--text-primary);
        background: radial-gradient(120% 120% at 0% 0%, #1e3a8a 0%, #020617 55%);
        min-height: 100vh;
        display: flex;
        align-items: stretch;
      }

      a {
        color: var(--accent);
        text-decoration: none;
        transition: color 0.2s ease, background-color 0.2s ease;
      }

      a:hover {
        color: #0ea5e9;
      }

      .layout {
        display: flex;
        width: 100%;
      }

      .sidebar {
        position: sticky;
        top: 0;
        height: 100vh;
        width: var(--nav-width);
        padding: 3rem 2rem;
        display: flex;
        flex-direction: column;
        gap: 3rem;
        background: linear-gradient(
          180deg,
          rgba(15, 23, 42, 0.85) 0%,
          rgba(15, 23, 42, 0.55) 100%
        );
        border-right: 1px solid rgba(100, 116, 139, 0.25);
        backdrop-filter: blur(16px);
      }

      .brand h1 {
        margin: 0;
        font-size: 1.75rem;
        font-weight: 700;
      }

      .brand p {
        margin: 0.5rem 0 0;
        color: var(--text-secondary);
        line-height: 1.5;
      }

      .nav-links {
        display: flex;
        flex-direction: column;
        gap: 1rem;
        padding: 0;
        margin: 0;
        list-style: none;
      }

      .nav-links a {
        display: block;
        padding: 0.75rem 1rem;
        border-radius: 0.85rem;
        background-color: transparent;
        font-weight: 500;
        color: var(--text-secondary);
        border: 1px solid transparent;
      }

      .nav-links a:hover,
      .nav-links a:focus {
        color: var(--text-primary);
        background-color: rgba(56, 189, 248, 0.12);
        border-color: rgba(56, 189, 248, 0.25);
      }

      main {
        flex: 1;
        padding: 3.5rem clamp(2rem, 4vw, 5rem);
        display: flex;
        flex-direction: column;
        gap: var(--gap);
      }

      section {
        display: flex;
        flex-direction: column;
        gap: 1.75rem;
      }

      section h2 {
        margin: 0 0 0.75rem;
        font-size: 1.6rem;
        letter-spacing: 0.02em;
        text-transform: uppercase;
        color: var(--muted);
      }

      .section-card {
        background: var(--surface);
        border-radius: 1.75rem;
        padding: 2.5rem;
        border: 1px solid rgba(148, 163, 184, 0.15);
        box-shadow: 0 25px 60px -35px rgba(15, 23, 42, 0.8);
        backdrop-filter: blur(18px);
      }

      .intro-heading {
        font-size: clamp(2.5rem, 5vw, 3.75rem);
        line-height: 1.1;
        margin: 0;
      }

      .intro-subtitle {
        font-size: 1.1rem;
        color: var(--text-secondary);
        margin: 1rem 0 2rem;
        max-width: 52ch;
        line-height: 1.6;
      }

      .cta-group {
        display: flex;
        flex-wrap: wrap;
        gap: 1rem;
      }

      .cta-group a {
        display: inline-flex;
        align-items: center;
        justify-content: center;
        gap: 0.5rem;
        padding: 0.9rem 1.4rem;
        border-radius: 999px;
        border: 1px solid rgba(148, 163, 184, 0.35);
        color: var(--text-primary);
        background: rgba(56, 189, 248, 0.08);
        font-weight: 500;
      }

      .cta-group a.primary {
        background: linear-gradient(135deg, #38bdf8, #2563eb);
        border-color: transparent;
      }

      .cta-group a:hover {
        border-color: rgba(56, 189, 248, 0.55);
        transform: translateY(-1px);
      }

      .experience-list {
        display: flex;
        flex-direction: column;
        gap: 1.5rem;
        padding: 0;
        margin: 0;
        list-style: none;
      }

      .experience-item {
        position: relative;
        padding-left: 1.75rem;
      }

      .experience-item::before {
        content: "";
        position: absolute;
        left: 0;
        top: 0.35rem;
        width: 0.65rem;
        height: 0.65rem;
        border-radius: 50%;
        background: var(--accent);
        box-shadow: 0 0 0 6px rgba(56, 189, 248, 0.1);
      }

      .experience-item h3 {
        margin: 0;
        font-size: 1.15rem;
      }

      .experience-item .meta {
        margin: 0.35rem 0;
        color: var(--muted);
      }

      .experience-item p {
        margin: 0;
        color: var(--text-secondary);
        line-height: 1.6;
      }

      .detail-list {
        margin: 0.75rem 0 0;
        padding-left: 1.15rem;
        display: flex;
        flex-direction: column;
        gap: 0.6rem;
        color: var(--text-secondary);
      }

      .detail-list li {
        line-height: 1.55;
      }

      .cards-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
        gap: 1.4rem;
      }

      .feedback-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
        gap: 1.5rem;
      }

      .card {
        background: var(--surface-strong);
        border-radius: 1.25rem;
        padding: 1.75rem;
        border: 1px solid rgba(148, 163, 184, 0.15);
        display: flex;
        flex-direction: column;
        gap: 0.75rem;
        transition: transform 0.2s ease, box-shadow 0.2s ease;
      }

      .card:hover {
        transform: translateY(-6px);
        box-shadow: 0 25px 50px -25px rgba(56, 189, 248, 0.35);
      }

      .card h3 {
        margin: 0;
        font-size: 1.2rem;
      }

      .card p {
        margin: 0;
        color: var(--text-secondary);
        line-height: 1.55;
      }

      .card .meta {
        font-size: 0.9rem;
        color: var(--muted);
      }

      .card .card-link {
        align-self: flex-start;
        margin-top: 0.25rem;
        font-weight: 600;
      }

      .repo-stats {
        display: flex;
        align-items: center;
        gap: 0.75rem;
        margin-top: 0.5rem;
        color: var(--text-secondary);
        font-size: 0.95rem;
      }

      .repo-stats .label {
        color: var(--muted);
        font-weight: 500;
      }

      .feature-list {
        margin: 0;
        padding-left: 1.1rem;
        display: flex;
        flex-direction: column;
        gap: 0.45rem;
        color: var(--text-secondary);
        font-size: 0.95rem;
      }

      .skill-groups {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
        gap: 1.5rem;
      }

      .skill-group h3 {
        margin: 0;
        font-size: 1.05rem;
        color: var(--text-primary);
      }

      .pill-list {
        margin: 0.75rem 0 0;
        padding: 0;
        list-style: none;
        display: flex;
        flex-wrap: wrap;
        gap: 0.5rem;
      }

      .pill-list li {
        padding: 0.35rem 0.75rem;
        border-radius: 999px;
        background: rgba(148, 163, 184, 0.15);
        color: var(--text-secondary);
        font-size: 0.9rem;
      }

      .languages {
        margin-top: 2rem;
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
        gap: 1rem;
      }

      .language-card {
        padding: 1.25rem 1.5rem;
        border-radius: 1rem;
        border: 1px solid rgba(148, 163, 184, 0.15);
        background: rgba(15, 23, 42, 0.6);
      }

      .language-card h3 {
        margin: 0;
        font-size: 1rem;
        color: var(--text-primary);
      }

      .language-card p {
        margin: 0.3rem 0 0;
        color: var(--text-secondary);
        font-size: 0.95rem;
      }

      blockquote {
        margin: 0;
        padding: 2rem;
        border-radius: 1.5rem;
        border: 1px solid rgba(148, 163, 184, 0.18);
        background: rgba(15, 23, 42, 0.8);
        position: relative;
      }

      blockquote p {
        margin: 0 0 1.5rem;
        font-size: 1.05rem;
        color: var(--text-secondary);
        line-height: 1.7;
      }

      blockquote footer {
        font-weight: 600;
        color: var(--text-primary);
      }

      @media (max-width: 1200px) {
        :root {
          --nav-width: 240px;
        }
      }

      @media (max-width: 1024px) {
        body {
          flex-direction: column;
        }

        .sidebar {
          position: static;
          height: auto;
          width: 100%;
          flex-direction: column;
          align-items: flex-start;
          gap: 2rem;
          padding: 2rem clamp(1.5rem, 4vw, 3rem);
          border-right: none;
          border-bottom: 1px solid rgba(100, 116, 139, 0.25);
        }

        .nav-links {
          flex-direction: row;
          flex-wrap: wrap;
          gap: 0.75rem;
        }

        .nav-links a {
          padding: 0.7rem 1rem;
        }

        main {
          padding: 2.5rem clamp(1.5rem, 5vw, 3.5rem);
        }
      }

      @media (max-width: 640px) {
        .cta-group {
          flex-direction: column;
        }

        section h2 {
          font-size: 1.25rem;
        }

        .section-card {
          padding: 2rem;
        }
      }
    </style>
  </head>
  <body>
    <div class="layout">
      <aside class="sidebar">
        <div class="brand">
          <h1>Hassan Wasfy</h1>
          <p>
            Mobile Software Engineer based in Helwan, Cairo. I design resilient
            Android platforms with a clean architecture mindset and a focus on
            measurable impact.
          </p>
        </div>
        <nav>
          <ul class="nav-links">
            <li><a href="#intro">Intro</a></li>
            <li><a href="#experience">Experience</a></li>
            <li><a href="#apps">Apps</a></li>
            <li><a href="#libraries">Libraries</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#feedback">Feedback</a></li>
          </ul>
        </nav>
      </aside>

      <main>
        <section id="intro">
          <div class="section-card">
            <h2>Intro</h2>
            <h3 class="intro-heading">Building robust Android products with intent</h3>
            <p class="intro-subtitle">
              Experienced Android developer with 3+ years crafting secure,
              scalable mobile applications. Comfortable across Kotlin, Java, and
              Jetpack ecosystems — from architecting MVVM/MVI flows to shipping
              polished UX with Compose, and partnering with teams to deliver
              measurable business results.
            </p>
            <div class="cta-group">
              <a class="primary" href="https://wa.me/+201508043285" target="_blank" rel="noreferrer">WhatsApp</a>
              <a href="https://www.linkedin.com/in/hassanwasfy7/" target="_blank" rel="noreferrer">LinkedIn</a>
              <a href="mailto:hassanwasfy7@gmail.com" target="_blank" rel="noreferrer">Email</a>
              <a href="https://t.me/aboHarroun" target="_blank" rel="noreferrer">Telegram</a>
            </div>
          </div>
        </section>

        <section id="experience">
          <div class="section-card">
            <h2>Experience</h2>
            <ul class="experience-list">
              <li class="experience-item">
                <h3>Tasheel Info Tech · Mid-Senior Android Developer</h3>
                <p class="meta">Mar 2024 — Present · Full-time · Hybrid</p>
                <ul class="detail-list">
                  <li>
                    Delivered a secure authenticator app with biometric login,
                    encrypted storage, and real-time OTP sync over Ktor WebSockets.
                  </li>
                  <li>
                    Architected an offline-first ECM solution using Room, custom
                    caching, and Jetpack Compose to streamline document workflows.
                  </li>
                  <li>
                    Drove clean MVVM structure with Kotlin + Hilt/Koin, ensuring
                    scalable code and smooth hand-offs with backend and QA teams.
                  </li>
                </ul>
              </li>
              <li class="experience-item">
                <h3>Ultimate Solutions Egy · Android Developer</h3>
                <p class="meta">Mar 2024 — Dec 2024 · Full-time · On-site</p>
                <ul class="detail-list">
                  <li>
                    Rebuilt legacy Distribution v8 IX architecture from scratch,
                    moving to MVVM and modern design patterns (Adapter, Builder,
                    Facade, Singleton).
                  </li>
                  <li>
                    Revamped six core business screens and introduced Favorites
                    and Recents, boosting usability across 7 global markets.
                  </li>
                  <li>
                    Reduced technical debt by refreshing 85% of critical code and
                    improving overall performance and stability.
                  </li>
                </ul>
              </li>
              <li class="experience-item">
                <h3>Twerlo UAE · Android Developer</h3>
                <p class="meta">May 2024 — Dec 2024 · Part-time · Remote</p>
                <ul class="detail-list">
                  <li>
                    Implemented Clean Architecture foundations and reusable,
                    testable components aligned with evolving product flows.
                  </li>
                  <li>
                    Delivered features across Activities, Fragments, Services, and
                    background workers while migrating key screens to Compose.
                  </li>
                  <li>
                    Partnered with design, backend, and QA to ship reliable
                    releases and resolve performance regressions.
                  </li>
                </ul>
              </li>
              <li class="experience-item">
                <h3>Desh &amp; Dezz · Android Developer</h3>
                <p class="meta">Aug 2023 — Dec 2023 · Full-time · Remote</p>
                <ul class="detail-list">
                  <li>
                    Built a custom chat feature library and integrated secure API
                    endpoints with the backend team.
                  </li>
                  <li>
                    Improved crash-free users from 44% to 87% by eliminating
                    memory leaks and stabilizing release builds.
                  </li>
                  <li>
                    Boosted home screen performance by 65% through targeted
                    profiling and optimizations.
                  </li>
                </ul>
              </li>
              <li class="experience-item">
                <h3>iSchool · Software Programming Instructor</h3>
                <p class="meta">Mar 2024 — Apr 2024 · Part-time · Remote</p>
                <ul class="detail-list">
                  <li>
                    Mentored students aged 6–18 on core software concepts and
                    game development fundamentals.
                  </li>
                  <li>
                    Crafted age-appropriate curricula that made programming
                    approachable and practical.
                  </li>
                </ul>
              </li>
              <li class="experience-item">
                <h3>Law Office · Android Developer</h3>
                <p class="meta">Sep 2022 — Feb 2023 · Full-time · On-site</p>
                <ul class="detail-list">
                  <li>
                    Delivered a bespoke case-management app covering clients,
                    finances, scheduling, and event tracking for legal teams.
                  </li>
                </ul>
              </li>
            </ul>
          </div>
        </section>

        <section id="apps">
          <div class="section-card">
            <h2>Personal Apps</h2>
            <div class="cards-grid">
              <article class="card">
                <h3>Dev Assist</h3>
                <p>
                  AI-powered productivity companion that tracks career progress,
                  surfaces learning insights, and embeds Gemini-driven chat for
                  developers.
                </p>
                <p class="meta">Stack: MVVM · Coroutines · Retrofit · Hilt · Compose · Room</p>
              </article>
              <article class="card">
                <h3>BeepBeep</h3>
                <p>
                  Platform of six apps spanning riders, restaurants, taxi partners,
                  and support teams — all orchestrated with real-time APIs and
                  synchronized dashboards.
                </p>
                <p class="meta">Stack: KMM · Coroutines · Ktor · Jetpack Compose · Realm DB</p>
                <a href="https://github.com/TheChance101/beep-beep" target="_blank" rel="noreferrer">View on GitHub</a>
              </article>
              <article class="card">
                <h3>IMOVE</h3>
                <p>
                  Immersive movie discovery experience delivering rich details,
                  pagination, and offline access with a modern Android architecture.
                </p>
                <p class="meta">Stack: Coroutines · Pagination · Ktor · Jetpack Compose · Room</p>
                <a href="https://github.com/RedVelvet-Team/IMovie" target="_blank" rel="noreferrer">View on GitHub</a>
              </article>
              <article class="card">
                <h3>CashierMe</h3>
                <p>
                  Offline-first point-of-sale app linked to a remote control panel,
                  enabling instant invoicing, automatic migrations, and rich
                  business dashboards.
                </p>
                <p class="meta">Google Play · Kotlin · Offline sync · Custom analytics</p>
              </article>
            </div>
          </div>
        </section>

        <section id="libraries">
          <div class="section-card">
            <h2>Personal Libraries</h2>
            <div class="cards-grid">
              <article class="card">
                <h3>LocalizeMe</h3>
                <p>
                  Lightweight localization toolkit that lets Android apps switch
                  languages on the fly across XML and Compose experiences.
                </p>
                <p class="meta">Focus: Runtime Locale Switching · 33+ Locales · Currency &amp; Digit Helpers</p>
                <ul class="feature-list">
                  <li>LanguageManager API swaps locales without restarts.</li>
                  <li>Ships 33+ locale presets plus currency formatting utilities.</li>
                  <li>Digit normalization bridges Arabic-Indic and ASCII flows.</li>
                </ul>
                <div class="repo-stats" data-repo="hassanwasfy/LocalizeMe">
                  <span><span class="label">Stars</span> ⭐ <span class="value">—</span></span>
                  <span><span class="label">Forks</span> 🍴 <span class="value">—</span></span>
                </div>
                <a class="card-link" href="https://github.com/hassanwasfy/LocalizeMe" target="_blank" rel="noreferrer">View on GitHub</a>
              </article>
              <article class="card">
                <h3>ScreenTracker</h3>
                <p>
                  Lifecycle-aware tracker that records active Activities and
                  Fragments, designed for analytics and debugging visibility.
                </p>
                <p class="meta">Focus: Automatic Screen Logging · WeakReference Safety · Firebase Hooks</p>
                <ul class="feature-list">
                  <li>Initializes once in `Application` to monitor app navigation.</li>
                  <li>Offers instant access to the current screen name for logs or BI.</li>
                  <li>Optional Firebase integration for production analytics.</li>
                </ul>
                <div class="repo-stats" data-repo="hassanwasfy/iTell">
                  <span><span class="label">Stars</span> ⭐ <span class="value">—</span></span>
                  <span><span class="label">Forks</span> 🍴 <span class="value">—</span></span>
                </div>
                <a class="card-link" href="https://github.com/hassanwasfy/iTell" target="_blank" rel="noreferrer">View documentation</a>
              </article>
              <article class="card">
                <h3>DialogMe</h3>
                <p>
                  Highly customizable dialog builder supporting XML apps and
                  Compose screens with consistent design tokens.
                </p>
                <p class="meta">Focus: Animated Dialogs · Multi-button Actions · Compose &amp; XML APIs</p>
                <ul class="feature-list">
                  <li>Configurable titles, messages, icons, and button palettes.</li>
                  <li>Compose API mirrors classic setup for shared theming.</li>
                  <li>Ships with polished entrance/exit animations out of the box.</li>
                </ul>
                <div class="repo-stats" data-repo="hassanwasfy/DialogMe">
                  <span><span class="label">Stars</span> ⭐ <span class="value">—</span></span>
                  <span><span class="label">Forks</span> 🍴 <span class="value">—</span></span>
                </div>
                <a class="card-link" href="https://github.com/hassanwasfy/DialogMe" target="_blank" rel="noreferrer">View on GitHub</a>
              </article>
            </div>
          </div>
        </section>

        <section id="skills">
          <div class="section-card">
            <h2>Skills</h2>
            <div class="skill-groups">
              <article class="skill-group">
                <h3>Core Languages &amp; UI</h3>
                <ul class="pill-list">
                  <li>Kotlin</li>
                  <li>Java</li>
                  <li>Jetpack Compose</li>
                  <li>XML</li>
                  <li>Android SDK</li>
                </ul>
              </article>
              <article class="skill-group">
                <h3>Architecture &amp; Patterns</h3>
                <ul class="pill-list">
                  <li>Clean Architecture</li>
                  <li>MVC</li>
                  <li>MVP</li>
                  <li>MVVM</li>
                  <li>Design Patterns</li>
                </ul>
              </article>
              <article class="skill-group">
                <h3>Tooling &amp; Analytics</h3>
                <ul class="pill-list">
                  <li>Git &amp; GitHub</li>
                  <li>Firebase</li>
                  <li>Crashlytics</li>
                  <li>Google Analytics</li>
                  <li>Push Notifications</li>
                </ul>
              </article>
              <article class="skill-group">
                <h3>Platform Capabilities</h3>
                <ul class="pill-list">
                  <li>RESTful APIs</li>
                  <li>DI (Hilt · Koin)</li>
                  <li>Room</li>
                  <li>Work Manager</li>
                  <li>Coroutine Utilization</li>
                </ul>
              </article>
              <article class="skill-group">
                <h3>Testing &amp; Quality</h3>
                <ul class="pill-list">
                  <li>JUnit4</li>
                  <li>JUnit5</li>
                  <li>UI/UX Standards</li>
                  <li>Android UI Principles</li>
                </ul>
              </article>
            </div>
            <div class="languages">
              <div class="language-card">
                <h3>Arabic</h3>
                <p>Native</p>
              </div>
              <div class="language-card">
                <h3>English</h3>
                <p>Excellent</p>
              </div>
            </div>
          </div>
        </section>

        <section id="feedback">
          <div class="section-card">
            <h2>Clients Feedback</h2>
            <div class="feedback-grid">
              <blockquote>
                <p>
                  “Hassan transformed our authentication stack into a secure,
                  biometric-first experience while keeping delivery ahead of
                  schedule.”
                </p>
                <footer>— Product Manager, Tasheel Info Tech</footer>
              </blockquote>
              <blockquote>
                <p>
                  “He rebuilt Distribution v8 IX with modern architecture,
                  shrinking legacy debt and giving our teams the velocity we
                  needed.”
                </p>
                <footer>— Product Lead, Ultimate Solutions Egy</footer>
              </blockquote>
              <blockquote>
                <p>
                  “Crash-free sessions jumped to 87% after Hassan’s fixes. His
                  focus on quality and performance made a measurable difference.”
                </p>
                <footer>— CTO, Desh &amp; Dezz</footer>
              </blockquote>
            </div>
          </div>
        </section>
      </main>
    </div>
    <script>
      const fetchRepoStats = async (repoId, container) => {
        try {
          const response = await fetch(`https://api.github.com/repos/${repoId}`);
          if (!response.ok) throw new Error(`Status ${response.status}`);
          const data = await response.json();
          const valueSpans = container.querySelectorAll(".value");
          if (valueSpans.length >= 2) {
            valueSpans[0].textContent = data.stargazers_count ?? "0";
            valueSpans[1].textContent = data.forks_count ?? "0";
          }
        } catch (error) {
          console.error(`Failed to fetch stats for ${repoId}`, error);
          const valueSpans = container.querySelectorAll(".value");
          valueSpans.forEach((span) => (span.textContent = "N/A"));
        }
      };

      const repoStatBlocks = document.querySelectorAll(".repo-stats");
      repoStatBlocks.forEach((block) => {
        const repoId = block.getAttribute("data-repo");
        if (repoId) {
          fetchRepoStats(repoId, block);
        }
      });
    </script>
  </body>
</html>
