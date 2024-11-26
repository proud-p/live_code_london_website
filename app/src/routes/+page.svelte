<div class="container">
    <div class="title-banner">
      <h1 class="title"> Live Code London </h1>
      <section class="next-event">

        <h2>Upcoming Event</h2>
        <br/>
        <p>Placeholder for next upcoming event</p>
    </section>
    
    </div>
  
    <div class="menu-items">
      <nav>
	<a href="/">Home</a>
    <a href="/resources">Resources</a>
	<a href="/about">About</a>
	
	<a href="/events">Events</a>
	<a href="/donate">Donate</a>
	<a href="/faq">FAQ</a>
  </nav>
    </div>
  </div>
  
  <style>
    .title {
      font-family: 'ZillaSlabHighlight';
      padding: 5%;
      font-size: 3rem;
    }

    /* Main container styling for full screen */
    .container {
      display: flex;
      height: 100vh;
      flex-direction: row; /* Default: side by side */
    }
  
    /* Common styling for both title-banner and menu-items */
    .title-banner, .menu-items {
      width: 50%;            /* Each takes up half the width on larger screens */
      display: flex;          /* Flexbox for child alignment */
      flex-direction: column;
      justify-content: center; /* Center vertically */
      align-items: center;     /* Center horizontally */
      padding: 5%;
      border: white 3px solid;
    }
  
    .title-banner {
      text-align: center;
      margin: 1% 0.5% 1% 1%;
    }
  
    .menu-items {
        margin: 1% 1% 1% 0.5%;
    }
    

.menu-items nav a {
    display: block;
    color: rgba(255, 255, 255, 0.95);
    text-decoration: none;
    margin: 5px 0;
    font-size: 2rem;
    padding-left: 20px;   /* Space for the ">" symbol */
    position: relative;   /* Needed for absolute positioning of ::before */
    width: 40%;         /* Set a fixed width to prevent shifting */
    text-align: left;     /* Align text to the left within each link */
    font-family: 'KodeMono';
}

.menu-items nav a:hover {
  color: black;
  background-color: white;
  transition: 0.2s ease;
  width: auto;
}

.menu-items nav a:hover::before {
    content: "> ";
    color: black;
    background-color: white;
    position: absolute;
    left: 0;
   
}

.next-event {
  margin: 5%;
}



    .next-event p{
      padding: 10%;
      border: 2px white solid;
     
    }
  
    /* Media query to stack items on smaller screens */
    @media (max-width: 768px) {
      .container {
        flex-direction: column; /* Stack top to bottom on small screens */
      }
  
      .title-banner,
      .menu-items {
        width: 100%; /* Take full width in stacked layout */
        height: 50vh; /* Take half the height in stacked layout */
      }
    }
  </style>
  