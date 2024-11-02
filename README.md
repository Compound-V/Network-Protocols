
# Networking Basics Webpage

This project showcases a simple webpage about the basics of networking, including common protocols, ports, and uses. This webpage is designed using HTML and CSS and can be hosted on GitHub Pages to be shared with others.

## Table of Contents

- [Getting Started](#getting-started)
- [Setup Instructions](#setup-instructions)
- [Creating the HTML and CSS Files](#creating-the-html-and-css-files)
- [Publishing on GitHub Pages](#publishing-on-github-pages)
- [Updating Your Site](#updating-your-site)

## Getting Started

These instructions will help you set up a simple HTML and CSS webpage and publish it using GitHub Pages.

## Setup Instructions

1. **Create a New GitHub Repository**:
   - Go to [GitHub](https://github.com/) and log in to your account.
   - Click on the **+** icon in the top-right corner and select **New repository**.
   - Name the repository (e.g., `networking-basics`), set it to **Public**, and click **Create repository**.

2. **Clone the Repository Locally** (optional if you want to work locally):
   ```bash
   git clone https://github.com/yourusername/networking-basics.git
   cd networking-basics
   ```

## Creating the HTML and CSS Files

1. **Create `index.html`**:
   - In the repository folder, create a file named `index.html` and add the following content:

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Basics of Networking</title>
       <link rel="stylesheet" href="styles.css">
   </head>
   <body>
       <div class="container">
           <h1>Basics of Networking</h1>
           <p class="intro">
               A network is a collection of interconnected devices that communicate and share resources using a set of defined protocols over a common transmission medium.
           </p>
           <p class="definition">
               Networking is the process of connecting various devices so that they can communicate with each other and share information and resources.
           </p>
           <p class="protocols">
               Network protocols are sets of rules or standards used by devices to communicate with each other over a network.
           </p>
           <p class="layers">
               Network protocols can be broadly categorized into "layers". Each layer relies on the layer below it and provides services to the layer above it.
           </p>
           <p>This table covers the most essential protocols across networking layers and use cases:</p>
           
           <table>
               <thead>
                   <tr>
                       <th>Protocol</th>
                       <th>Use</th>
                       <th>Port(s)</th>
                       <th>Standard</th>
                   </tr>
               </thead>
               <tbody>
                   <tr>
                       <td>HTTP</td>
                       <td>Web browsing</td>
                       <td>80</td>
                       <td>RFC 2616, RFC 7230-7235</td>
                   </tr>
                   <tr>
                       <td>HTTPS</td>
                       <td>Secure web browsing</td>
                       <td>443</td>
                       <td>RFC 2818, RFC 5246 (TLS)</td>
                   </tr>
                   <tr>
                       <td>FTP</td>
                       <td>File transfer</td>
                       <td>20 (Data), 21 (Control)</td>
                       <td>RFC 959</td>
                   </tr>
                   <!-- Add more rows as needed -->
               </tbody>
           </table>
       </div>
   </body>
   </html>
   ```

2. **Create `styles.css`**:
   - In the same folder, create a file named `styles.css` and add the following content:

   ```css
   /* styles.css */
   body {
       font-family: Arial, sans-serif;
       background-color: #1a1a1a;
       color: #f0f0f0;
       margin: 0;
       padding: 0;
   }

   .container {
       max-width: 800px;
       margin: auto;
       padding: 20px;
   }

   h1 {
       font-size: 2em;
       color: #f0f0f0;
   }

   .intro, .definition, .protocols, .layers {
       margin: 10px 0;
       line-height: 1.6;
   }

   table {
       width: 100%;
       border-collapse: collapse;
       margin-top: 20px;
   }

   table, th, td {
       border: 1px solid #333;
   }

   th, td {
       padding: 12px;
       text-align: left;
   }

   thead {
       background-color: #333;
       color: #f0f0f0;
   }

   tbody tr:nth-child(even) {
       background-color: #282828;
   }

   tbody tr:hover {
       background-color: #3d3d3d;
   }

   p.intro {
       color: #d1453b; /* Red */
   }

   p.definition {
       color: #32b875; /* Green */
   }

   p.protocols {
       color: #31a1f2; /* Blue */
   }

   p.layers {
       color: #cccccc; /* Light Gray */
   }
   ```

## Publishing on GitHub Pages

1. Go to your repository on GitHub.
2. Click on **Settings**.
3. In the **Code and automation** section, select **Pages**.
4. Under **Source**, choose **Deploy from a branch**.
5. Select `main` (or `master`) as the branch and `/root` as the directory, then click **Save**.

Your page will be live at `https://yourusername.github.io/networking-basics/` after a few moments.

## Updating Your Site

To make changes:
1. Edit your files locally.
2. Commit and push to GitHub:

   ```bash
   git add .
   git commit -m "Update content"
   git push
   ```

GitHub Pages will automatically update your site.

---

Happy Coding!
