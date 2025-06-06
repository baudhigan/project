# Project Responsive Web Design using Bootstrap
# Date: 20.05.2025
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
```

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Dribbble Clone</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
  <style>
    body {
      background-color: #f8f9fa;
    }
    .project-card {
      border: 1px solid #dee2e6;
      border-radius: 8px;
      overflow: hidden;
      background: #fff;
    }
    .project-card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }
    .project-info {
      padding: 15px;
    }
    .search-bar {
      max-width: 400px;
      margin: 0 auto;
    }
  </style>
</head>
<body>

<!-- Navbar -->
<nav class="navbar navbar-light bg-light px-4">
  <img src="dribblogo.png">
  <div>
    <button class="btn btn-outline-dark me-2" data-bs-toggle="modal" data-bs-target="#loginModal">Login</button>
    <button class="btn btn-dark" data-bs-toggle="modal" data-bs-target="#signupModal">Sign Up</button>
  </div>
</nav>

<!-- Header -->
<div class="text-center my-4">
  <h1>Discover the world's top designers</h1>
  <p class="text-muted">Explore work from the most talented and accomplished designers ready to take on your next project.</p>
  <div class="search-bar input-group mb-3">
    <input type="text" class="form-control" placeholder="What are you looking for?" />
    <button class="btn btn-outline-secondary">Search</button>
  </div>
</div>

<!-- Projects -->
<div class="container">
  <h4>Popular Projects</h4>
  <div class="row g-4 mt-2">
    <!-- Card 1 -->
    <div class="col-md-4">
      <div class="project-card">
        <img src="dri1.png" alt="Geometries" />
        <div class="project-info">
          <h6>Geometries</h6>
          <p class="text-muted small">A project on geometric designs.</p>
        </div>
      </div>
    </div>
    <!-- Card 2 -->
    <div class="col-md-4">
      <div class="project-card">
        <img src="dri2.png" alt="Low Poly Designs" />
        <div class="project-info">
          <h6>Low Poly Designs</h6>
          <p class="text-muted small">A project on low poly designs.</p>
        </div>
      </div>
    </div>
    <!-- Card 3 -->
    <div class="col-md-4">
      <div class="project-card">
        <img src="original-280a1bebac9b2d7533888b031a1ed9a5.webp" alt="Conspiracies" />
        <div class="project-info">
          <h6>Conspiracies</h6>
          <p class="text-muted small">A project on conspiracies.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="row g-4 mt-2">
    <!-- Card 1 -->
    <div class="col-md-4">
      <div class="project-card">
        <img src="teo.webp" alt="Geometries" />
        <div class="project-info">
          <h6>Geometries</h6>
          <p class="text-muted small">A project on geometric designs.</p>
        </div>
      </div>
    </div>
    <!-- Card 2 -->
    <div class="col-md-4">
      <div class="project-card">
        <img src="dri 6.png" alt="Low Poly Designs" />
        <div class="project-info">
          <h6>Low Poly Designs</h6>
          <p class="text-muted small">A project on low poly designs.</p>
        </div>
      </div>
    </div>
    <!-- Card 3 -->
    <div class="col-md-4">
      <div class="project-card">
        <img src="dri5.png" alt="Conspiracies" />
        <div class="project-info">
          <h6>Conspiracies</h6>
          <p class="text-muted small">A project on conspiracies.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Login Modal -->
<div class="modal fade" id="loginModal" tabindex="-1" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content p-4">
      <div class="modal-header">
        <h5 class="modal-title">Login</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
      </div>
      <div class="modal-body">
        <form>
          <div class="mb-3">
            <label for="loginUserID" class="form-label">User ID</label>
            <input type="text" class="form-control" id="loginUserID" placeholder="Enter your user ID" />
          </div>
          <div class="mb-3">
            <label for="loginPassword" class="form-label">Password</label>
            <input type="password" class="form-control" id="loginPassword" placeholder="Enter your password" />
          </div>
          <button type="submit" class="btn btn-dark w-100">Login</button>
        </form>
      </div>
    </div>
  </div>
</div>

<!-- Sign Up Modal -->
<div class="modal fade" id="signupModal" tabindex="-1" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content p-4">
      <div class="modal-header">
        <h5 class="modal-title">Sign Up</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
      </div>
      <div class="modal-body">
        <form>
          <div class="mb-3">
            <label for="fullName" class="form-label">Full Name</label>
            <input type="text" class="form-control" id="fullName" placeholder="Enter your full name" />
          </div>
          <div class="mb-3">
            <label for="address" class="form-label">Address</label>
            <input type="text" class="form-control" id="address" placeholder="Enter your address" />
          </div>
          <div class="mb-3">
            <label for="dob" class="form-label">Date of Birth</label>
            <input type="date" class="form-control" id="dob" />
          </div>
          <div class="mb-3">
            <label for="signupUserID" class="form-label">User ID</label>
            <input type="text" class="form-control" id="signupUserID" placeholder="Create a user ID" />
          </div>
          <div class="mb-3">
            <label for="signupPassword" class="form-label">Password</label>
            <input type="password" class="form-control" id="signupPassword" placeholder="Create a password" />
          </div>
          <button type="submit" class="btn btn-dark w-100">Sign Up</button>
        </form>
      </div>
    </div>
  </div>
</div>

<!-- Bootstrap JS -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>

</body>
<br><br>
<footer style="background-color:rgb(58, 58, 58);height: 150;width: 1600px;color: white;text-align: center;font-family: cursive;font-size: 5;margin-top:30;">
    <h2 style="font-size:medium; margin-top: 4;">Email : dribbble@gmail.com </h2> <h2 style="font-size:medium;">Contact number : +71 566640000</h2><br>
    <h2 style="font-size:medium;">Address  : No 4/7, High's Street ,Banglore Highway ,Chennai</h2>
    <br>
    <h2 style="font-size:medium;">----------Developed by BAUDHIGAN D--------- </h2>
</footer>
</html>

```
# OUTPUT:
![Alt text](<Screenshot 2025-05-20 104349.png>)
![Alt text](<Screenshot 2025-05-20 104358.png>)
![Alt text](<Screenshot 2025-05-20 104408.png>)
![Alt text](<Screenshot 2025-05-20 104419.png>)
# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
