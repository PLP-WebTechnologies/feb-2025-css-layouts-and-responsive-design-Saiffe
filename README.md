# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]Include at least:
>  - navigation bar
>  - media queries
>  - 

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.
- <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Responsive Layout with Navigation</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <nav>
      <ul class="navbar">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main class="container">
    <section class="box">Box 1</section>
    <section class="box">Box 2</section>
    <section class="box">Box 3</section>
    <section class="box">Box 4</section>
  </main>

  <footer>
    <p>&copy; 2025 Your Website</p>
  </footer>
</body>
</html>
CSS 
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background-color: #f0f0f0;
}

header {
  background-color: #333;
  color: white;
  padding: 1rem;
}

.navbar {
  display: flex;
  justify-content: center;
  list-style: none;
}

.navbar li {
  margin: 0 1rem;
}

.navbar a {
  color: white;
  text-decoration: none;
  font-weight: bold;
  padding: 0.5rem;
  transition: background-color 0.3s ease;
}

.navbar a:hover {
  background-color: #4CAF50;
  border-radius: 5px;
}

.container {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: center;
  padding: 2rem;
}

.box {
  background-color: #ffffff;
  border: 1px solid #ddd;
  padding: 2rem;
  flex: 1 1 calc(25% - 1rem);
  text-align: center;
}

footer {
  background-color: #333;
  color: white;
  padding: 1rem;
  text-align: center;
}

/* Responsive Design */
@media (max-width: 1024px) {
  .box {
    flex: 1 1 calc(33.33% - 1rem);
  }
}

@media (max-width: 768px) {
  .box {
    flex: 1 1 calc(50% - 1rem);
  }

  .navbar {
    flex-direction: column;
  }

  .navbar li {
    margin: 0.5rem 0;
  }
}

@media (max-width: 480px) {
  .box {
    flex: 1 1 100%;
  }

  .navbar {
    flex-direction: column;
    align-items: center;
  }

  .navbar li {
    margin: 0.5rem 0;
  }
}


Happy Coding! 💻✨
