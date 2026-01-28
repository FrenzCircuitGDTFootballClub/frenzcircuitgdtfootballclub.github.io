<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Frenz Circuit GDT Football Club</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    body {
      min-height: 100vh;
      overflow-x: hidden;
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
      color: white;
    }

    /* Flying footballs */
    .football {
      position: absolute;
      font-size: 2.5rem;
      animation: fly linear infinite;
      opacity: 0.7;
      z-index: 1;
    }

    @keyframes fly {
      from {
        transform: translateX(-10vw) rotate(0deg);
      }
      to {
        transform: translateX(110vw) rotate(360deg);
      }
    }

    .football:nth-child(1) { top: 15%; animation-duration: 12s; }
    .football:nth-child(2) { top: 35%; animation-duration: 9s; }
    .football:nth-child(3) { top: 55%; animation-duration: 14s; }
    .football:nth-child(4) { top: 75%; animation-duration: 11s; }

    /* Main content */
    .content {
      position: relative;
      z-index: 2;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 40px 20px;
    }

    h1 {
      font-size: 3rem;
      letter-spacing: 2px;
    }

    .tagline {
      margin: 10px 0 30px;
      font-size: 1.2rem;
      opacity: 0.9;
    }

    /* Contact box */
    .contact {
      margin-top: 30px;
      background: rgba(0, 0, 0, 0.35);
      padding: 25px 30px;
      border-radius: 15px;
      max-width: 420px;
      width: 100%;
    }

    .contact h2 {
      margin-bottom: 15px;
      font-size: 1.6rem;
    }

    .contact p {
      margin: 8px 0;
      font-size: 1rem;
    }

    .contact a {
      color: #00ffcc;
      text-decoration: none;
      font-weight: bold;
    }

    .contact a:hover {
      text-decoration: underline;
