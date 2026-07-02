# Blog-platform-

  <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Blog Platform</title>
<link rel="stylesheet" href="style.css">
</head>
<body>

<header>
<div class="logo">Blog Platform</div>

<nav>
<a href="index.html">Home</a>
<a href="login.html">Login</a>
<a href="register.html">Register</a>
<a href="dashboard.html">Dashboard</a>
</nav>
</header>

<section class="hero">
<h1>Welcome to Blog Platform</h1>
<p>Create, share and discuss ideas with everyone.</p>

<a href="register.html" class="btn">Get Started</a>
</section>

<section class="features">

<div class="card">
<h2>Create Posts</h2>
<p>Create and publish your blogs instantly.</p>
</div>

<div class="card">
<h2>Comments</h2>
<p>Interact through comments and discussions.</p>
</div>

<div class="card">
<h2>Secure Login</h2>
<p>JWT based authentication system.</p>
</div>

</section>

<footer>
<p>© 2026 Blog Platform | Full Stack Development Project</p>
</footer>

</body>
</html>
<!DOCTYPE html>
<html>
<head>
<title>Login</title>
<link rel="stylesheet" href="style.css">
</head>

<body>

<div class="form-container">

<h2>Login</h2>

<form id="loginForm">

<input type="email"
placeholder="Email"
id="email"
required>

<input type="password"
placeholder="Password"
id="password"
required>

<button type="submit">
Login
</button>

<p>
Don't have an account?
<a href="register.html">Register</a>
</p>

</form>

</div>

<script src="script.js"></script>

</body>
</html>

<!DOCTYPE html>
<html>

<head>

<title>Register</title>

<link rel="stylesheet"
href="style.css">

</head>

<body>

<div class="form-container">

<h2>Create Account</h2>

<form id="registerForm">

<input
type="text"
placeholder="Full Name"
id="name"
required>

<input
type="email"
placeholder="Email"
id="email"
required>

<input
type="password"
placeholder="Password"
id="password"
required>

<button type="submit">
Register
</button>

<p>

Already have account?

<a href="login.html">
Login
</a>

</p>

</form>

</div>

<script src="script.js"></script>

</body>
</html>

<!DOCTYPE html>

<html>

<head>

<title>Dashboard</title>

<link
rel="stylesheet"
href="style.css">

</head>

<body>

<header>

<h1>
My Dashboard
</h1>

<a href="index.html">
Home
</a>

</header>

<div class="container">

<h2>Create Blog</h2>

<form id="postForm">

<input
type="text"
id="title"
placeholder="Blog Title"
required>

<textarea
id="content"
placeholder="Write your blog..."
required>
</textarea>

<button
type="submit">
Publish
</button>

</form>

<hr>

<div id="posts">

<!-- Blog posts appear here -->

</div>

</div>

<script src="script.js"></script>

</body>
</html>



