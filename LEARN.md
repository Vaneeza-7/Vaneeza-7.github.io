# LEARN.md

## How I Built My Portfolio 🎨

Welcome to the guide on how I built my personal portfolio. This document will walk you through detailed steps and technologies I used.

### Table of Contents

1. [Project Setup](#project-setup)
2. [HTML Structure](#html-structure)
3. [Styling with CSS](#styling-with-css)
4. [Interactive Elements with JavaScript](#interactive-elements-with-javascript)
5. [Utilizing Bootstrap](#utilizing-bootstrap)
6. [Final Touches](#final-touches)

### Project Setup

1. **Creating the Repository**: I started by creating a new repository on GitHub named `vaneeza-7.github.io`. This name ensures that GitHub Pages will host my portfolio.
   
     <i>Note: Please make sure that you write your own username, like this `yourusername.github.io`</i>
   

3. **Cloning the Repository**: I cloned the repository to my local machine using the command:
    ```sh
    git clone https://github.com/Vaneeza-7/vaneeza-7.github.io.git
    ```

4. **Setting Up the Project Structure**: I created the basic folder structure:
    ```
    vaneeza-7.github.io/
    ├── index.html
    ├── css/
    │   └── styles.css
    ├── js/
    │   └── scripts.js
    └── assets/
        ├── images/
        └── fonts/
    ```

### HTML Structure

1. **Creating `index.html`**: This is the main file that contains the structure of my portfolio. Here’s a snippet of how I structured the HTML:
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Vaneeza Ahmad - Portfolio</title>
        <link rel="stylesheet" href="css/styles.css">
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    </head>
    <body>
        <header>
            <nav class="navbar navbar-expand-lg navbar-light bg-light">
                <a class="navbar-brand" href="#">Vaneeza Ahmad</a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNav">
                    <ul class="navbar-nav ml-auto">
                        <li class="nav-item active">
                            <a class="nav-link" href="#about">About</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#projects">Projects</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#contact">Contact</a>
                        </li>
                    </ul>
                </div>
            </nav>
        </header>
        <main>
            <!-- Content will go here -->
        </main>
        <footer>
            <p>&copy; 2024 Vaneeza Ahmad</p>
        </footer>
        <script src="js/scripts.js"></script>
    </body>
    </html>
    ```

### Styling with CSS

1. **Creating `styles.css`**: In the `css` folder, I created `styles.css` to handle the styling of the portfolio. Here are some key styles I used:
    ```css
    body {
        font-family: 'Arial', sans-serif;
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    header {
        background: #f8f9fa;
        padding: 10px 0;
        box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    footer {
        text-align: center;
        padding: 10px 0;
        background: #f8f9fa;
        position: fixed;
        width: 100%;
        bottom: 0;
    }
    ```

### Interactive Elements with JavaScript

1. **Creating `scripts.js`**: In the `js` folder, I created `scripts.js` to handle the interactive elements of the portfolio. For example, I added smooth scrolling for navigation links:
    ```javascript
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function(e) {
            e.preventDefault();

            document.querySelector(this.getAttribute('href')).scrollIntoView({
                behavior: 'smooth'
            });
        });
    });
    ```

### Utilizing Bootstrap

1. **Adding Bootstrap**: I used Bootstrap to make my portfolio responsive and visually appealing. Here’s how I integrated it:
    - Added Bootstrap CDN in the `<head>` section of `index.html`.
    - Used Bootstrap classes for layout and components, such as `navbar`, `container`, `row`, and `col`.

2. **Example**: Here’s an example of a Bootstrap grid layout for the projects section:
    ```html
    <section id="projects" class="container">
        <h2>Projects</h2>
        <div class="row">
            <div class="col-md-4">
                <div class="card">
                    <img src="assets/images/project1.jpg" class="card-img-top" alt="Project 1">
                    <div class="card-body">
                        <h5 class="card-title">Project 1</h5>
                        <p class="card-text">Description of Project 1.</p>
                        <a href="#" class="btn btn-primary">View Project</a>
                    </div>
                </div>
            </div>
            <!-- Repeat for more projects -->
        </div>
    </section>
    ```

### Final Touches

1. **Testing and Deployment**: After building and styling my portfolio, I thoroughly tested it across different devices and screen sizes to ensure it was responsive.

2. **Deploying on GitHub Pages**: I pushed my changes to the `main` branch of the GitHub repository. GitHub Pages automatically deployed the site.

   <i> Note: you would need to enable github actions in the repository settings for this step. </i>

3. **Continuous Updates**: I continue to update my portfolio with new projects and improvements. 

Feel free to explore the code, suggest improvements, or ask any questions!

Happy coding!

---

Vaneeza
