# coursera-html-css-js
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>My Module 2 Solution</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <h1>Our Menu</h1>
  <div class="section">Chicken</div>
  <div class="section">Beef</div>
  <div class="section">Sushi</div>
</body>
</html>


/* Base styles */
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  padding: 20px;
  font-family: Arial, sans-serif;
}

h1 {
  text-align: center;
  font-size: 2.5em;
  margin-bottom: 30px;
}

.container {
  width: 100%;
  overflow: hidden;
}

.box {
  position: relative;
  background-color: #f2f2f2;
  border: 1px solid black;
  padding: 50px 15px 15px 15px; /* Push down text from top */
  margin: 10px;
}

.section-title {
  position: absolute;
  top: 0;
  right: 0;
  padding: 5px 15px;
  border: 1px solid black;
  font-size: 1.25em;
  font-weight: bold;
  color: #fff;
}

/* Section-specific colors */
.chicken {
  background-color: #ff6666;
}

.beef {
  background-color: #cc6600;
}

.sushi {
  background-color: #339999;
}

/* Desktop view (≥ 992px) */
@media (min-width: 992px) {
  .box {
    float: left;
    width: 33.33%;
  }
}

/* Tablet view (768px–991px) */
@media (min-width: 768px) and (max-width: 991px) {
  .box {
    float: left;
    width: 50%;
  }
  .box:nth-child(3) {
    width: 100%;
  }
}

/* Mobile view (≤ 767px) */
@media (max-width: 767px) {
  .box {
    width: 100%;
  }
}

