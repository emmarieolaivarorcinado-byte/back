<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Print Xpress | Printing Services</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
      color: #333;
      min-height: 100vh;
    }

    header {
      background: linear-gradient(135deg, #003366 0%, #004080 100%);
      color: white;
      padding: 30px 0;
      text-align: center;
      box-shadow: 0 10px 30px rgba(0,51,102,0.3);
      position: sticky;
      top: 0;
      z-index: 100;
    }

    header h1 {
      font-size: 2.5rem;
      margin-bottom: 5px;
      letter-spacing: 2px;
      text-transform: uppercase;
      font-weight: 700;
    }

    header p {
      font-size: 1.1rem;
      opacity: 0.95;
      font-weight: 300;
    }

    nav {
      background: linear-gradient(90deg, #004080 0%, #005fa3 100%);
      display: flex;
      justify-content: center;
      gap: 40px;
      padding: 15px;
      flex-wrap: wrap;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }

    nav a {
      color: white;
      text-decoration: none;
      font-weight: 600;
      transition: all 0.3s ease;
      position: relative;
      font-size: 1rem;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    nav a::after {
      content: '';
      position: absolute;
      bottom: -5px;
      left: 0;
      width: 0;
      height: 3px;
      background: #ffcc00;
      transition: width 0.3s ease;
    }

    nav a:hover {
      color: #ffcc00;
      transform: translateY(-2px);
    }

    nav a:hover::after {
      width: 100%;
    }

    .hero {
      background: linear-gradient(135deg, #003366 0%, #004080 100%);
      height: 70vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      color: white;
      text-shadow: 2px 2px 10px rgba(0,0,0,0.5);
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle, rgba(255,204,0,0.1) 1px, transparent 1px);
      background-size: 50px 50px;
      animation: float 20s linear infinite;
    }

    @keyframes float {
      0% { transform: translate(0, 0); }
      100% { transform: translate(50px, 50px); }
    }

    .hero h2 {
      font-size: 3.5rem;
      margin-bottom: 20px;
      font-weight: 800;
      position: relative;
      z-index: 2;
      animation: slideDown 0.8s ease;
    }

    .hero p {
      font-size: 1.5rem;
      position: relative;
      z-index: 2;
      font-weight: 300;
      animation: slideUp 0.8s ease;
    }

    @keyframes slideDown {
      from {
        opacity: 0;
        transform: translateY(-30px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes slideUp {
      from {
        opacity: 0;
        transform: translateY(30px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .container {
      max-width: 1200px;
      margin: 50px auto;
      padding: 20px;
    }

    .section-title {
      text-align: center;
      color: #003366;
      font-size: 2.5rem;
      margin-bottom: 50px;
      position: relative;
      padding-bottom: 20px;
    }

    .section-title::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 50%;
      transform: translateX(-50%);
      width: 100px;
      height: 5px;
      background: linear-gradient(90deg, transparent, #ffcc00, transparent);
      border-radius: 10px;
    }

    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 30px;
      margin-bottom: 50px;
    }

    .card {
      background: white;
      border-radius: 16px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.1);
      overflow: hidden;
      transition: all 0.4s ease;
      position: relative;
    }

    .card::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255,204,0,0.2), transparent);
      transition: left 0.5s ease;
      z-index: 1;
    }

    .card:hover::before {
      left: 100%;
    }

    .card:hover {
      transform: translateY(-15px) rotateX(5deg);
      box-shadow: 0 20px 50px rgba(0,0,0,0.2);
    }

    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      transition: transform 0.4s ease;
    }

    .card:hover img {
      transform: scale(1.1);
    }

    .card-content {
      padding: 25px;
      position: relative;
      z-index: 2;
    }

    .card h3 {
      color: #003366;
      font-size: 1.5rem;
      margin-bottom: 15px;
      font-weight: 700;
    }

    .card 
