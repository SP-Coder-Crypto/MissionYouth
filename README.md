<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Mission Community Youth Center Inc. — a non-profit providing programs and services for children and families." />
  <title>Mission Community Youth Center Inc.</title>

  <style>
    :root {
      --bg: #b6afA4; /* original RGB converted */
      --accent: #8e5311;
      --accent-strong: #7e5a0e;
      --accent-hover: #d08f0e;
      --text: #513f03;
      --container-max: 1100px;
      --radius: 12px;
      --nav-height: 56px;
    }

    /* Basic reset */
    * {
      box-sizing: border-box;
    }

    html, body {
      height: 100%;
      margin: 0;
      padding: 0;
      background-color: var(--bg);
      color: var(--text);
      font-family: Arial, Helvetica, sans-serif;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height: 1.6;
    }

    /* Centered page container */
    .site {
      max-width: var(--container-max);
      margin: 0 auto;
      padding: 0 20px 40px;
    }

    /* Skip link (for keyboard users) */
    .skip-link {
      position: absolute;
      left: -999px;
      top: auto;
      width: 1px;
      height: 1px;
      overflow: hidden;
    }
    .skip-link:focus {
      left: 10px;
      top: 10px;
      width: auto;
      height: auto;
      padding: 8px 12px;
      background: #000;
      color: #fff;
      z-index: 9999;
      border-radius: 4px;
      text-decoration: none;
    }

    header {
      text-align: center;
      padding: 24px 0;
    }

    header h1 {
      font-size: clamp(24px, 4vw, 40px);
      color: #60440a;
      margin: 0;
    }

    /* Navigation */
    nav {
      background-color: var(--accent);
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 6px rgba(0,0,0,0.12);
    }

    nav .nav-inner {
      display: flex;
      gap: 8px;
      align-items: center;
      justify-content: center;
      max-width: var(--container-max);
      margin: 0 auto;
      padding: 6px 12px;
    }

    nav a {
      display: inline-block;
      color: #ffffff;
      text-align: center;
      padding: 10px 14px;
      text-decoration: none;
      font-size: 16px;
      border-radius: 6px;
    }

    nav a:hover,
    nav a:focus {
      background-color: var(--accent-hover);
      color: #fff;
      outline: none;
    }

    /* Main content */
    main#main {
      background: transparent;
      padding: 28px 12px;
      margin-top: 12px;
      font-size: clamp(16px, 1.25vw, 20px);
      text-align: left;
      color: var(--text);
    }

    .hero-image {
      width: 100%;
      max-width: 500px;
      height: auto;
      display: block;
      margin: 28px auto;
      border-radius: var(--radius);
      object-fit: cover;
      box-shadow: 0 4px 12px rgba(0,0,0,0.08);
      background: #fff;
    }

    .main-para {
      font-weight: 600;
    }

    footer {
      background-color: var(--accent-strong);
      color: white;
      text-align: center;
      padding: 12px;
      margin-top: 32px;
      border-radius: 6px;
    }

    /* Responsive tweaks */
    @media (max-width: 640px) {
      nav .nav-inner {
        flex-wrap: wrap;
        padding: 8px;
      }
      nav a {
        padding: 8px 10px;
        font-size: 15px;
      }
      .site {
        padding: 0 12px 30px;
      }
      header {
        padding: 18px 0;
      }
    }
  </style>
</head>

<body>
  <a class="skip-link" href="#main">Skip to content</a>

  <div class="site">
    <!-- HEADER -->
    <header>
      <h1>Mission Community Youth Center Inc.</h1>
    </header>

    <!-- NAVIGATION -->
    <nav role="navigation" aria-label="Main navigation">
      <div class="nav-inner">
        <!-- Note: GitHub Pages is case-sensitive. Ensure these filenames match files in your repo. -->
        <a href="MissionHome.html">Home</a>
        <a href="enrollment.html">Enrollment</a>
        <a href="about.html">About Us</a>
        <a href="contact.html">Contact</a>
        <a href="events.html">Events</a>
      </div>
    </nav>

    <!-- MAIN CONTENT -->
    <main id="main" role="main" aria-labelledby="site-title">
      <p class="main-para">
        Mission Community Youth Center Inc. is a non-profit organization dedicated to providing a safe,
        supportive, and enriching environment for children and families in our community. We offer a wide
        range of programs and services designed to foster growth, learning, and development in a fun and
        engaging way.
      </p>

      <!-- Make sure mission-logo.jpeg exists in the repository root (case-sensitive) -->
      <img class="hero-image" src="mission-logo.jpeg" alt="Mission Community Youth Center logo" />
    </main>

    <!-- FOOTER -->
    <footer>
      <p>&copy; 2026 Mission Community Youth Center Inc. | Privacy Policy | Terms of Service</p>
    </footer>
  </div>
</body>

</html>
