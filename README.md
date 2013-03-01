#HTML, CSS

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

###Table
    
    <table>
      <tr>
        <th>Heading</th>
        <th>Heading</th>
      </tr>
      <tr>
        <td>Data</td>
        <td>★★★</td>
      </tr>
      <tr>
        <td>Data</td>
        <td>★★★★</td>
      </tr>
    </table>

    table {
      width: 100%;
    }
    table th,
    table td {
      padding: 10px 20px;
      text-align: left;
      border-bottom: 1px solid #ccc;
    }
    table th {
      border-width: 2px;
    }
    table td {
      color: #666;
    }
    table tr:last-child th,
    table tr:last-child td {
      border-bottom: none;
    }
    table tr:nth-child(even) {
      background: #eee;
    }
    
    
    
    
    
    
#Responsive

    // IPHONE LANDSCAPE
    @media screen and (max-device-width: 480px), screen and (max-width: 480px) {
    
    }

    // IPHONE PORTRAIT
    @media screen and (max-device-width: 400px), screen and (max-width: 400px) {
    
    }

##Neat SCSS includes

    @include outer-container;
#
    @include span-columns(6);

The last column in a row

    @include omega(); 

A column fills up half of a column  

    @include span-columns(3 of 6); 
