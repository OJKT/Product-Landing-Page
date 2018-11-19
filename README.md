# Product-Landing-Page
FCC Challenge 3 cert 1
<style>
@import 'https://fonts.googleapis.com/css?family=Allerta+Stencil';

* {
  margin: 0px;
  padding: 10px;
  box-sizing: border-box;
}

#page-wrapper {
  position: relative;
}

body {
  background-color: #CCFFFF;
  font-family: 'Lato', sans-serif;
}

li {
  list-style: none;
}

a {
  color: #000;
  text-decoration: none;
}

/** global classes styling **/

.container {
  max-width: 1000px;
  width: 100%;
  margin: auto;
}

.btn {
  padding: 0 20px;
  height: 40px;
  font-size: 1em;
  font-weight: 900;
  text-transform: uppercase;
  border: 3px black solid;
  border-radius: 2px;
  background: transparent;
  cursor: pointer;
}

.grid {
  display: flex;
}

// navigation bar

header {
  position: fixed;
  top: 0px;
	left: 0px;
  min-height: 8px;
	padding: 0 20px;
  display: flex;
  align-items: ceter;
  background-color: #330019;
	justify-content: space-around;
  @media (max-width: 1000px) {
    flex-wrap: wrap;
  }
}

.logo {
  width: 5vw;
  
  @media (max-width: 650px) {
    margin-top: 20px;
    width: 100%;
    position: relative;
  }
  
  img {
    width: 100%;
    height: 100%;
    max-width: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    margin-left: 20px;
    @media (max-width: 650px) {
      margin: 0 auto;
    }
  }
}

nav {
  font-weight: 400;
  
  @media (max-width: 650px) {
    margin-top: 10px;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    padding: 50px;
		text-color: white;
    
    li {
     padding-bottom: 5px; 
    }
  }
  
  ul {
    width: 35vw;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    
    @media (max-width: 650px) {
      flex-direction: column;
    }
  }
}

// hero

#hero {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  height: 200px;
  margin-top: 90px;
	
  h2 {
		margin-top: 40px;
    margin-bottom: 20px;
    word-wrap: break-word;
		font-family: 'Allerta Stencil', sans-serif;
		font-size: 40px;
		font-color: black;
  }

  input[type="email"] {
    max-width: 275px;
    width: 100%;
    padding: 5px;
  }

  input[type="submit"] {
    max-width: 150px;
    width: 100%;
    height: 30px;
    margin: 15px 0;
    border: 0;
    background-color: orange;
		font-family: 'Allerta Stencil', sans-serif;
    
    &:hover {
      background-color: yellow;
      transition: background-color 1s;
    }
  }
  
  @media (max-width: 650px) {
    margin-top: 120px;
  }
}

// features

#features {
  margin-top: 30px;
  .icon {
    display: flex;
    align-items: right;
    justify-content: center;
    height: 125px;
    width: 20vw;
    color: orange;
		font-family: 'Allerta Stencil', sans-serif;
		}

    @media (max-width: 550px) {
      display: none;
			font-family: 'Allerta Stencil', sans-serif;
    }
  }

  .desc {
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 125px;
    width: 80vw;
    padding: 5px;
		font-family: 'Allerta Stencil', sans-serif;

    @media (max-width: 550px) {
      width: 100%;
      text-align: center;
      padding: 0;
      height: 150px;
			font-family: 'Allerta Stencil', sans-serif;
    }
  
  @media (max-width: 650px) {
    margin-top: 0;
		font-family: 'Allerta Stencil', sans-serif;
  }
}

// how it works

#how-it-works {
  margin-top: 50px;
  display: flex;
  justify-content: center;
  
  iframe {
    max-width: 560px;
    width: 100%;
  }
}

// pricing

#pricing {
  margin-top: 60px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  
	.hr {
		margin-top: 15px;
	}
	
  #tenor, #bass, #valve {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    width: calc(100%  / 3);
    margin: 10px;
    border: 1px solid #000;
    border-radius: 3px;
		font-family: 'Allerta Stencil', sans-serif;
		background-color: #C0C0C0;
    
    .level {
      background-color: black;
      color: orange;
      padding: 15px 0;
      width: 100%;
      text-transform: uppercase;
      font-weight: 700;
    }
    
    h2 {
      margin-top: 50px;
    }
    
    ol {
      margin: 15px 0;
			color: white;
      
      li { padding: 5px 0; }
    }
    
    button {
      border: 0;
      margin: 15px 0;
      background-color: #f1c40f;
      font-weight: 400;
      
      &:hover {
        background-color: orange;
        transition: background-color 1s;
      }
    }
  }
  
  @media (max-width: 800px) {
    flex-direction: column;
    
    #tenor, #bass, #valve { max-width: 300px; width: 100%; margin: 0 auto; margin-bottom: 10px; }
  }
}

// footer

footer {
  margin-top: 30px;
	margin-bottom: 15px;
  background-color: #C0C0C0;
  padding: 10px;
	border: 1px solid #000;
 	border-radius: 10px;
	}
  
  ul {
    display: flex;
    justify-content: flex-end;
		background-color: #808080;
		margin-left: 40px;
	}
    
 		li {
      padding: 8px;
			margin: 5px;
			border-radius: 4px;
			padding: 15px;
			padding-left: 20px;
			padding-right: 20px;
    }
  
  span {
    margin-top: 10px;
    display: flex;
    justify-content: flex-end;
    font-size: 0.9em;
    color: #444;
  }
</style>
<div id="page-wrapper">
<header id="header">
  <div class="logo">
    <img id="header-img" src="https://scontent-lhr3-1.xx.fbcdn.net/v/t1.0-9/10259912_1433065623614416_4016796773353521076_n.png?_nc_cat=109&_nc_ht=scontent-lhr3-1.xx&oh=7782ab9207bb08e7a5597e2b67c2341f&oe=5C82FB82" alt="original trombones logo" />
  </div>

  <nav id="nav-bar">
    <ul>
      <li font-color: white><a class="nav-link" href="#features">Features</a></li>
      <li><a class="nav-link" href="#how-it-works">How It Works</a></li>
      <li><a class="nav-link" href="#pricing">Pricing</a></li>
    </ul>
  </nav>

</header>

<div class="container">

</div>

<section id="hero">
  <h2>Handcrafted Masterpieces</h2>
  <form id="form" action="#">
    <input name="email" id="email" type="email" placeholder="Enter your email address" required/>
    <input id="submit" type="submit" value="Get Started" class="btn"></input>
  </form>
</section>


<div class="container">
	<hr>
  <section id="features">
    <div class="grid">
      <div class="icon">
        <i class="fa fa-3x fa-fire"></i>
      </div>
      <div class="desc">
        <h2>Premium Materials</h2>
        <p>Our Longboards use the best hardwoods which is sourced locally. This will increase the quality of your purchase.</p>
      </div>
    </div>
		<hr>
    <div class="grid">
      <div class="icon">
        <i class="fa fa-3x fa-truck"></i>
      </div>
      <div class="desc">
        <h2>Fast Shipping</h2>
        <p>We make sure you recieve your longboard as soon as we have finished making it. We also provide free returns if you are not satisfied.</p>
      </div>
    </div>
		<hr>
    <div class="grid">
      <div class="icon">
        <i class="fa fa-3x fa-battery-full" aria-hidden="true"></i>
      </div>
      <div class="desc">
        <h2>Quality Assurance</h2>
        <p>For every purchase you make, we will ensure there are no damages or faults and we will check and test the pitch of your instrument.</p>
      </div>
    </div>
		<hr>
  </section>
  <section id="how-it-works">
    <iframe id="video" height="315" src="https://ak6.picdn.net/shutterstock/videos/23582566/preview/stock-footage-beutiful-and-soft-pink-pastel-lighning-at-winter-time-following-camera-with-close-up-on-skater.webm" frameborder="0" allowfullscreen></iframe>
  </section>
  <section id="pricing">
    <div id="tenor">
      <div class="level">
        Long <br>Board
      </div>
      <h2>$600</h2>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
      <button class="btn">Select</button>
    </div>
    <div id="bass">
      <div class="level">
        Longer <br>board
      </div>
      <h2>$900</h2>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
      <button class="btn">Select</button>
    </div>
    <div id="valve">
      <div class="level">
        Longest <br>Board
      </div>
      <h2>$1200</h2> 
        <li>lorum ipsum.</li>
        <li>lorem ipsum.</li>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
      <button class="btn">Select</button>
    </div>
  </section>
  <footer>
		<ul>
      <li><a href="#">Privacy</a></li>
      <li><a href="#">Terms</a></li>
      <li><a href="https://www.facebook.com/Active-Boardom-1433050133615965/?__tn__=kC-R&eid=ARDxFnA2JMu6bjlwqWvI3V1d0Rce9HdYBzDGGtJp0BhH-ueOlTAQbh0whATwwgFna9sm9jkboRpjWJnD&hc_ref=ARQaDkOV-XEkdyZItVQH9yuafF_narIIMZukBWJoaFoVgKTTBr5qBLQ1pDtdCP1cxF0&fref=nf&__xts__[0]=68.ARDYkTx9CsRT4OGTCvkO4FfhIcApAmkjQ-zBxaLHt1nqutrcdBfuonVlBKBXLg-l6giN-MiLriy2iHhYK3-uZ7l8efaHcYfOQPPUo3YknyBCljz10jZVwawd_JPGlqxxUxpaKdDVOc7vv4zQb1gvTtbiga9MLXcGfadpQU6YN_ZFZFBORq0wTJ2gjwQWf-hqAyErVWR_HM-_tje583zlZDxOBvyFSIb71aWN5zby5u-Ar3tr-Zn6BXKJ03w-KH30lCsYY8yrgpdS7DWA_-M3ogU_9pI9jGXFww4iDR6qmOdznSinEPP_J0pCY3maDJ4_2n1-a3Uq57kDKz4vC98">Contact</a></li> <!--contact-->
		</ul>
    <span>&copy Copyright 2018, OJKT STYLES</span>
  </footer>
</div>
</div>
