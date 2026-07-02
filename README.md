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

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:#f4f7fb;
color:#333;
}

header{
display:flex;
justify-content:space-between;
align-items:center;
background:#1e88e5;
padding:15px 30px;
color:white;
}

.logo{
font-size:28px;
font-weight:bold;
}

nav a{
text-decoration:none;
color:white;
margin-left:20px;
font-weight:bold;
}

.hero{
text-align:center;
padding:80px 20px;
background:linear-gradient(135deg,#42a5f5,#1565c0);
color:white;
}

.hero h1{
font-size:45px;
margin-bottom:20px;
}

.hero p{
font-size:20px;
margin-bottom:30px;
}

.btn{
padding:12px 25px;
background:white;
color:#1565c0;
text-decoration:none;
border-radius:8px;
font-weight:bold;
}

.features{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
padding:40px;
}

.card{
background:white;
padding:25px;
border-radius:10px;
box-shadow:0 4px 10px rgba(0,0,0,.15);
}

.form-container{
width:380px;
margin:60px auto;
background:white;
padding:30px;
border-radius:10px;
box-shadow:0 0 15px rgba(0,0,0,.2);
}

.form-container h2{
text-align:center;
margin-bottom:20px;
}

input,textarea{
width:100%;
padding:12px;
margin:10px 0;
border:1px solid #ccc;
border-radius:5px;
font-size:16px;
}

textarea{
height:150px;
resize:none;
}

button{
width:100%;
padding:12px;
background:#1e88e5;
color:white;
border:none;
border-radius:5px;
cursor:pointer;
font-size:17px;
}

button:hover{
background:#1565c0;
}

.container{
width:90%;
max-width:1000px;
margin:30px auto;
}

.post{
background:white;
padding:20px;
margin-top:20px;
border-radius:10px;
box-shadow:0 2px 8px rgba(0,0,0,.15);
}

.post h3{
margin-bottom:10px;
}

.post p{
margin-bottom:15px;
}

.actions button{
width:auto;
margin-right:10px;
padding:8px 15px;
}

.comment{
background:#f2f2f2;
padding:10px;
margin-top:10px;
border-radius:5px;
}

.comment input{
margin-top:10px;
}

footer{
margin-top:40px;
background:#1e88e5;
color:white;
text-align:center;
padding:15px;
}


