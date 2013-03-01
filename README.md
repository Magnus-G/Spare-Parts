Spare-Parts
===========

###Baseline aligned texts, different size
    <span class="big">Big</span>
    <span class="small">Small</span>

    .big {
      font-size: 23px;
    }
    .small {
      font-size: 13px;
    }

###Fixed header

    <header>Fixed</header>

    header {
     width: 100%;
     background-color: black;
     color: white;
     position: fixed;
    }
    
###Sticky footer

    <div class="stickyfooter">
      <div class="content">
        ...content...
        <div class="push"></div>
      </div>
      <div class="footer"></div>
    </div>

    .stickyfooter {
      min-height: 100%;
      height:auto !important;
      height: 100%;
      margin: 0 auto -500px;
    }
    .footer {
      background-color: black;
      height: 500px;
    }
    .push {
     height: 500px;
    }
