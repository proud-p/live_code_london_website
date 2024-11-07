<div class="container">
    <div class="title-banner">
      <h1>Live Code London</h1>
      <section class="next-event">
        <h2>Next Upcoming Event</h2>
        <p>Placeholder for next upcoming event</p>
      </section>
    </div>
  
    <div class="menu-items">
      <p>Placeholder for menu items</p>
    </div>
  </div>
  
  <style>
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
  
    .next-event {
      margin-top: 10px;
     
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
  