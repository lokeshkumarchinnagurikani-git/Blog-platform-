<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>NEW C</title>

<link rel="stylesheet" href="style.css">

</head>

<body>

<header>

<div class="logo">
NEW C
</div>

<nav>

<a href="index.html">Home</a>

<a href="login.html">Login</a>

<a href="register.html">Register</a>

<a href="dashboard.html">Dashboard</a>

</nav>

</header>

<section class="hero">

<div class="overlay">

<h1 class="main-title">
NEW C
</h1>

<p class="sub-title">
Post the News Only
</p>

<a href="login.html" class="btn">
Login
</a>

<a href="register.html" class="btn">
Register
</a>

</div>

</section>

<section class="about">

<h2>
About NEW C
</h2>

<p>

NEW C is a simple online news platform where registered users can
publish news articles and allow readers to comment on them.
The platform provides secure login, easy news posting,
and an interactive comment system.

</p>

</section>

<section class="features">

<div class="card">

<h3>
📰 Post News
</h3>

<p>

Share the latest news with readers.

</p>

</div>

<div class="card">

<h3>
💬 Comments
</h3>

<p>

Readers can post comments and discuss news.

</p>

</div>

<div class="card">

<h3>
🔒 Secure Login
</h3>

<p>

Only registered users can post news.

</p>

</div>

</section>

<footer>

<p>

© 2026 NEW C | Post the News Only

</p>

</footer>

</body>

</html>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:#d9fdd3;
background-image:url("namaskar.jpg");
background-size:cover;
background-position:center;
background-attachment:fixed;
color:#222;
}

header{
display:flex;
justify-content:space-between;
align-items:center;
padding:18px 40px;
background:rgba(0,120,0,0.8);
}

.logo{
font-size:32px;
font-weight:bold;
color:white;
}

nav a{
color:white;
text-decoration:none;
margin-left:20px;
font-size:18px;
font-weight:bold;
}

nav a:hover{
color:yellow;
}

.hero{
height:90vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
}

.overlay{
background:rgba(0,0,0,.45);
padding:60px;
border-radius:15px;
}

.main-title{
font-size:70px;
color:white;
letter-spacing:5px;
margin-bottom:10px;
}

.sub-title{
font-size:22px;
font-style:italic;
color:#f5f5f5;
margin-bottom:30px;
}

.btn{
display:inline-block;
padding:12px 30px;
margin:10px;
background:#28a745;
color:white;
text-decoration:none;
border-radius:8px;
font-size:18px;
font-weight:bold;
transition:.3s;
}

.btn:hover{
background:#1b7d32;
}

.about{
width:90%;
max-width:1000px;
margin:40px auto;
padding:30px;
background:rgba(255,255,255,.9);
border-radius:12px;
text-align:center;
}

.about h2{
margin-bottom:15px;
color:#006400;
}

.features{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:25px;
width:90%;
margin:40px auto;
}

.card{
background:white;
padding:25px;
border-radius:12px;
box-shadow:0 5px 10px rgba(0,0,0,.2);
text-align:center;
transition:.3s;
}

.card:hover{
transform:translateY(-8px);
}

.card h3{
color:#0a7c2f;
margin-bottom:15px;
}

.form-container{
width:380px;
margin:60px auto;
background:rgba(255,255,255,.95);
padding:30px;
border-radius:12px;
box-shadow:0 5px 12px rgba(0,0,0,.2);
}

.form-container h2{
text-align:center;
margin-bottom:20px;
color:#006400;
}

input,textarea{
width:100%;
padding:12px;
margin:10px 0;
border:1px solid #aaa;
border-radius:6px;
font-size:16px;
}

textarea{
height:180px;
resize:none;
}

button{
width:100%;
padding:12px;
background:#28a745;
color:white;
border:none;
border-radius:6px;
font-size:18px;
cursor:pointer;
}

button:hover{
background:#1b7d32;
}

.post{
background:white;
padding:20px;
margin:20px auto;
width:90%;
border-radius:10px;
box-shadow:0 3px 8px rgba(0,0,0,.2);
}

.post h3{
color:#006400;
margin-bottom:10px;
}

.comment{
background:#eafbe7;
padding:10px;
margin-top:10px;
border-left:5px solid green;
border-radius:5px;
}

footer{
background:rgba(0,120,0,.8);
color:white;
text-align:center;
padding:18px;
margin-top:40px;
}

@media(max-width:768px){

header{
flex-direction:column;
}

nav{
margin-top:15px;
}

nav a{
display:block;
margin:10px 0;
}

.main-title{
font-size:45px;
}

.sub-title{
font-size:18px;
}

.overlay{
padding:35px;
}

}
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Login - NEW C</title>
<link rel="stylesheet" href="style.css">
</head>

<body>

<div class="form-container">

<h2>Customer Login</h2>

<form id="loginForm">

<input type="email"
id="loginEmail"
placeholder="Enter Email"
required>

<input type="password"
id="loginPassword"
placeholder="Enter Password"
required>

<button type="submit">
Login
</button>

<p style="text-align:center;margin-top:15px;">
Don't have an account?

<a href="register.html">
Register
</a>

</p>

</form>

</div>

<script src="script.js"></script>

</body>
</html>


<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport"
content="width=device-width, initial-scale=1.0">

<title>Register - NEW C</title>

<link rel="stylesheet"
href="style.css">

</head>

<body>

<div class="form-container">

<h2>Create Customer Account</h2>

<form id="registerForm">

<input
type="text"
id="name"
placeholder="Full Name"
required>

<input
type="email"
id="email"
placeholder="Email"
required>

<input
type="password"
id="password"
placeholder="Password"
required>

<button type="submit">

Register

</button>

<p style="text-align:center;margin-top:15px;">

Already Registered?

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
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport"
content="width=device-width, initial-scale=1.0">

<title>Dashboard - NEW C</title>

<link rel="stylesheet"
href="style.css">

</head>

<body>

<header>

<div class="logo">
NEW C
</div>

<nav>

<a href="index.html">
Home
</a>

<a href="#" onclick="logout()">
Logout
</a>

</nav>

</header>

<div class="container">

<h2 style="text-align:center;color:green;">
Post Today's News
</h2>

<form id="newsForm">

<input
type="text"
id="newsTitle"
placeholder="News Title"
required>

<textarea
id="newsContent"
placeholder="Write your news here..."
required></textarea>

<button type="submit">

Post News

</button>

</form>

<hr>

<div id="newsContainer">

<!-- News will appear here -->

</div>

</div>

<footer>

<p>

© 2026 NEW C | Post the News Only

</p>

</footer>

<script src="script.js"></script>

</body>
</html>
const registerForm=document.getElementById("registerForm");
const loginForm=document.getElementById("loginForm");
const newsForm=document.getElementById("newsForm");

let users=JSON.parse(localStorage.getItem("users"))||[];
let news=JSON.parse(localStorage.getItem("news"))||[];

if(registerForm){

registerForm.addEventListener("submit",function(e){

e.preventDefault();

const user={
name:document.getElementById("name").value,
email:document.getElementById("email").value,
password:document.getElementById("password").value
};

users.push(user);

localStorage.setItem("users",JSON.stringify(users));

alert("Registration Successful");

window.location="login.html";

});

}

if(loginForm){

loginForm.addEventListener("submit",function(e){

e.preventDefault();

let email=document.getElementById("loginEmail").value;
let password=document.getElementById("loginPassword").value;

let found=users.find(u=>u.email===email&&u.password===password);

if(found){

localStorage.setItem("currentUser",found.name);

alert("Login Successful");

window.location="dashboard.html";

}else{

alert("Invalid Email or Password");

}

});

}

if(newsForm){

displayNews();

newsForm.addEventListener("submit",function(e){

e.preventDefault();

const post={

title:document.getElementById("newsTitle").value,

content:document.getElementById("newsContent").value,

author:localStorage.getItem("currentUser"),

comments:[]

};

news.unshift(post);

localStorage.setItem("news",JSON.stringify(news));

newsForm.reset();

displayNews();

});

}

function displayNews(){

let container=document.getElementById("newsContainer");

if(!container) return;

container.innerHTML="";

news.forEach((post,index)=>{

container.innerHTML+=`

<div class="post">

<h3>${post.title}</h3>

<p>${post.content}</p>

<p><b>Posted By:</b> ${post.author}</p>

<input id="comment${index}" placeholder="Write a comment">

<button onclick="addComment(${index})">

Post Comment

</button>

<button onclick="editPost(${index})">

Edit

</button>

<button onclick="deletePost(${index})">

Delete

</button>

<div id="comments${index}">

${post.comments.map(c=>`<div class="comment">${c}</div>`).join("")}

</div>

</div>

`;

});

}

function addComment(index){

let box=document.getElementById("comment"+index);

if(box.value=="") return;

news[index].comments.push(box.value);

localStorage.setItem("news",JSON.stringify(news));

displayNews();

}

function editPost(index){

let newTitle=prompt("Edit Title",news[index].title);

let newContent=prompt("Edit Content",news[index].content);

if(newTitle!=null){

news[index].title=newTitle;

news[index].content=newContent;

localStorage.setItem("news",JSON.stringify(news));

displayNews();

}

}

function deletePost(index){

if(confirm("Delete this News?")){

news.splice(index,1);

localStorage.setItem("news",JSON.stringify(news));

displayNews();

}

}

function logout(){

localStorage.removeItem("currentUser");

window.location="login.html";

}



