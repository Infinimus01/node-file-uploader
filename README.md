<!-- // Import 'path' module to work with file and directory paths
const path = require("path");

// Import 'express' to create the web server
const express = require("express");

// Initialize the Express app
const app = express();

// Define the port number to run the server
const PORT = 3000;

// Middleware to parse incoming JSON requests (required for POST/PUT with JSON body)
app.use(express.json());

// Set EJS as the template/view engine (used to render dynamic HTML pages)
app.set("view engine", "ejs");

// Set the views directory (where .ejs files are stored)
app.set("views", path.resolve("./views"));

// Define a GET route for the homepage
app.get("/", (req, res) => {
  // Render the "homepage.ejs" file from the views folder
  return res.render("homepage");
});

// Start the server and listen on the defined port
app.listen(PORT, () => console.log(`server is running on port ${PORT}`)); -->
