<template>
<section>
<div class="wrap">
	<div class="about">
		<div class="about-intro">
			<h1 class="title">ABOUT</h1> 
      <br>
      
			<h3 class="sub-title">Let me introduce myself</h3>
			<div class="intro-details">
				<div class="intro-image">
					<div class="image">
						<img class="image-circle" src="../assets/jasoncalvert.png" alt="">
					</div>
				</div>
				<div class="intro-paragraph padding"><p>Lorem ipsum Exercitation culpa qui dolor consequat exercitation fugiat laborum ex ea eiusmod ad do aliqua occaecat nisi ad irure sunt id pariatur Duis laboris amet exercitation veniam labore consectetur ea id quis eiusmod.</p></div>
			</div>
		</div>
		<div class="about-info">
			<div class="profile padding">
				<h2 class="head">Profile</h2>
				<br><br><br>
				<div class="details">
				<h3>Fullname:</h3>
				<p>Ieuan Tomos Walker</p>
				<h3>Surname:</h3>
				<p>Mantini</p>
				<h3>Age:</h3>
				<p>26 years</p>
				<h3>Contact number:</h3>
				<p>067 065 3458</p>
				<h3>Email address:</h3>
				<p>liithamantini@gmail.com</p>
				<h3>Github account</h3>
				<p>GitRoss2021</p>
				<h3>Job:</h3>
				<p>Student</p>
				</div>
	
			</div>
			<div class="skills padding">
				<h2 class="head">Skills</h2>
			
				<ul class="skill-bars">
				   <li>
				   	<div class="progress percent90"><span>90%</span></div>
				   	<strong>HTML5</strong>
				   </li>
				   <li>
				   	<div class="progress percent85"><span>85%</span></div>
				   	<strong>CSS3</strong>
				   </li>
				   <li>
				   	<div class="progress percent70"><span>70%</span></div>
				   	<strong>JQuery</strong>
				   </li>
				   <li>
				   	<div class="progress percent95"><span>95%</span></div>
				   	<strong>PHP</strong>
				   </li>
				   <li>

				   	<div class="progress percent75"><span>75%</span></div>
				   	<strong>Wordpress</strong>
				   </li>
      
				</ul> <!-- /skill-bars -->		

				
			</div>
		</div>
		<div class="about-buttons padding">
			<div class="hire-me">
				<button class="about-button" href="/Contact">Hire me</button>
			</div>
			<!--  -->
		</div>
	</div>
</div>
</section>

</template>

<script>
import Navbar from '../components/Navbar.vue'
import Footer from '../components/Footer.vue'



export default {
 name: 'About', 
  components: {
    Navbar, Footer
  }
}
</script>

<style scoped>
 section{
   background-color: whitesmoke;
   height: 100vh;
   background: cover;
 }

*{
  font-family: "poppins-regular", sans-serif;
	box-sizing: border-box;
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
}

.about-intro{
  padding-top: 30px;
}

.image{
  height: 200px;
  width: 300px;
}

img{
  height: 200px;
  width: 350px;
}
.title{
  font-family: "poppins-regular", sans-serif;
}

.about-intro p{
  font-family: "poppins-regular", sans-serif;
  text-align: start;
  left: 20px;
}
.wrap{
	width: 100%;
	max-width: 1100px;
	height: 100%;
	margin: 0 auto;
	padding-left: 5px;
	padding-right: 5px;
}
.padding{
	padding: 4%;
}

/** Layout **/
.intro-details{
	display: -ms-flex;
    display: -webkit-flex;
    display: flex;
    flex-flow: row wrap;
}
	.intro-details > .intro-image{
	    width: 24%;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.intro-details > .intro-paragraph{
		width: 76%;
	}

.about-info{
	display: -ms-flex;
	display: -webkit-flex;
	display: flex;
	flex-direction: row;
}
	.about-info > .profile{
		-webkit-flex: 1 0 0;
   		flex: 1 0 0;
	}
	.about-info > .skills{
		-webkit-flex: 1 0 0;
   		flex: 1 0 0;
	}

.about-buttons{
	display: -ms-flex;
	display: -webkit-flex;
	display: flex;
	margin: 0 auto;
}
	.about-buttons div{
		width: 100%;
	}

/** Elements **/
.intro-image > .image{
	max-width: 60%;
	display: block;
	margin: 0 auto;
}
	.intro-image > .image > .image-circle{
		width: 100%;
		border-radius: 50%;
		margin: 0 auto;
		border: 5px solid #252439;
		transition: all .2s ease-in;
		-webkit-transition: all .2s ease-in;
		-moz-transition: all .2s ease-in;
		-o-transition: all .2s ease-in;
	}

.about-button{
	min-width: 70%;
	height: 100%;
	padding: 20px;
	font-family: "poppins-bold", sans-serif;
	text-align: center;
	text-transform: uppercase;
	letter-spacing: .3rem;
	cursor: pointer;
	font-size: 14px;
	transition: all .3s ease-in;
	-webkit-transition: all .3s ease-in;
	-moz-transition: all .3s ease-in;
	-o-transition: all .3s ease-in;
}
	.hire-me > .about-button{
		margin-right: 25px;
		float: right;
		color: #252439;
    	background-color: transparent;
		border: 3px solid #252439;
	}
		.hire-me > .about-button:hover{
			color: #1ed760;
			border-color: #1ed760;
		}
	.download-cv > .about-button{
		margin-left: 25px;
		color: #fff;
    	background-color: #252439;
		border: none;
		float: left;
	}
		.download-cv > .about-button:hover{
			background-color: #000;
		}

.skill-bars {
	list-style: none;
	margin: 6rem 0 3rem;
	padding: 0px;
}
.skill-bars li {
	height: .3rem;
	background: #a1a1a1;
	width: 100%;
	margin-bottom: 4rem;
	padding: 0;
	position: relative;
}
.skill-bars li strong {
	position: absolute;
	left: 0;
	top: -1rem;
	font-family: "poppins-bold", sans-serif;
	color: #252439;
	text-transform: uppercase;
	letter-spacing: .115rem;
	font-weight: normal;
	font-size: 16px;
	line-height: 0;
}
.skill-bars li .progress {
	background: #252439;
	position: relative;
	height: 100%;
}
.skill-bars li .progress span {
	position: absolute;
	right: 0;
	top: -3rem;
	display: block;
	font-family: "poppins-regular", sans-serif;
	color: white;
	font-size: 14px;
	line-height: 1;
	background: #252439;
	padding: .6rem .6rem;
	border-radius: 3px;
}
.skill-bars li .progress span::after {
	position: absolute;
	left: 50%;
	bottom: -5px;
	margin-left: -5px;
	border-right: 5px solid transparent;
	border-left: 5px solid transparent;
	border-top: 5px solid #313131;
	content: "";
}

.skill-bars li .percent5   { width: 5%; }
.skill-bars li .percent10  { width: 10%; }
.skill-bars li .percent15  { width: 15%; }
.skill-bars li .percent20  { width: 20%; }
.skill-bars li .percent25  { width: 25%; }
.skill-bars li .percent30  { width: 30%; }
.skill-bars li .percent35  { width: 35%; }
.skill-bars li .percent40  { width: 40%; }
.skill-bars li .percent45  { width: 45%; }
.skill-bars li .percent50  { width: 50%; }
.skill-bars li .percent55  { width: 55%; }
.skill-bars li .percent60  { width: 60%; }
.skill-bars li .percent65  { width: 65%; }
.skill-bars li .percent70  { width: 70%; }
.skill-bars li .percent75  { width: 75%; }
.skill-bars li .percent80  { width: 80%; }
.skill-bars li .percent85  { width: 85%; }
.skill-bars li .percent90  { width: 90%; }
.skill-bars li .percent95  { width: 95%; }
.skill-bars li .percent100 { width: 100%; }



/** Styles **/
.about h1, .about h2, .about h3, .about h4{
	color: #252439;
	font-family: "poppins-semibold", sans-serif;
}
.about h1, .about h4{
	font-family: serif;
	text-align: center;
}
.about h1{
	margin-top: 0px;
}
.about h4{
	color: #1ed760;
	letter-spacing: .25rem;
	margin-bottom: 8px;
	text-transform: uppercase;
}
.about h2{
	text-transform: uppercase;
	letter-spacing: .25rem;
	font-size: 19px;
}
.about h3{
	text-transform: uppercase;
	letter-spacing: .115rem;
	font-weight: normal;
	font-size: 16px;
	line-height: 0;
}
.about p{
	color: black;
	font-family: "lora-regular", serif;
	line-height: 1.5;
}
.intro-paragraph p{
	line-height: 1.8 !important;
	font-size: 20px;
}


/** Media Queries **/
@media all and (max-width : 800px) {
	.about-info{
		flex-direction: column;
	}
	.about-info h2{
		text-align: center;
	}
	.about-buttons{
		flex-direction: column;
	}
	.about-button{
		width: 100%;
	}
		.hire-me > .about-button{
			float: none;
			margin-right: 0px;
			margin-bottom: 15px;
		}
		.download-cv > .about-button{
			margin-left: 0px;	
			float: none;
		}
	.intro-image > .image {
		max-width: 95%;	
	}
	.intro-paragraph p{
		line-height: 1.5 !important;
		font-size: 18px;
	}
	.about h1 {
		font-size: 22px
	}
	.about h2, .about h3, .about h4{
		font-size: 15px
	}
}
@media all and (max-width : 500px) {
	.intro-details > .intro-image{
	    width: 100%;
	}
	.intro-details > .intro-paragraph{
		width: 100%;
		text-align: center;
	}
	.intro-image > .image{
		width: 40%;
	}
}

.details{
	text-align: start;
}

p{
	font-size: 17px;
}
.head{
	font-size: 31px !important;
}
</style>