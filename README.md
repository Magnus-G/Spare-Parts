#Variables

$base: 10px; 
<br>
$radius: 5px;
<br><br>

$default-color: gray;
<br>
$light-color: lighten($default-color, 20);
<br>
$dark-color: darken($default-color, 20);
<br>
$black-color: black;
<br>
$white-color: white;
<br>
$warning-color: yellow;
<br>
$important-color: red;
<br>








#HTML, CSS

###Dropdown menu

     <div class="dropdown">
          <a tabindex="1">Hover here</a>
          <ul>
                <li><a href="">Link</a></li>
                <li><a href="">Link</a></li>
          </ul>
     </div>
     

     .dropdown {
     
       a {
         cursor: pointer;
         position: relative;
       }
     
       &:hover ul {
         display: block;
       }
     
       ul { // dropdown
         display: none;
         left: 0px;
         position: absolute;
         padding: 10px;
         padding-bottom: 20px;
         background-color: gray;
         margin: 0;
     
         li {
           list-style: none;
           margin: 0;
     
           a { // each item in dropdown
             background-color: transparent;
             color: black;
             padding: 10px;
             width: 200px;
             &:hover {
               color: blue;
             }
           }
         }
       }
     }

###Button

###Button group

###Tabs

###Card
image, link, header, text, read more...

###Avatar & Comment

     <div class="comment">
      <div class="avatar"></div>
      <div>
        <h3>Name Lastname</h3>
        <h4>Timestamp</h4>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
      </div>
     </div>
     
     
    .comment {
      p {
        margin-left: 60px; // avatar width + margin-right
      }
      h3, h4 {
        display: inline;
      }
      .avatar {
        height: 50px;
        width: 50px;
        background-color: black;
        float: left;
        margin-right: 10px;
      }
    }

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
    
    
    
    
    
    
    
    
    
    
    
#Mixins

###Shadow

###Button
Sending in color

###Inset
Sending in color
    
    
    
    
    
    
    

#Animations

###Shake (TIL)
    
    
    
    
    
    
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
    
No margin gutters

    <div class="contain">
      <div class="table">
        <div class="column">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam neque officia dolorem</p>
        </div>
        <div class="column-last">
          <p>two</p>
        </div>
      </div>
    </div>


    .contain {
      @include outer-container;
    }
    
    .table {
      @include span-columns(12);
      @include row(table);
    }
    
    .column {
      @include span-columns(6, table);
      background-color: teal;
    }
    
    .column-last {
      @include span-columns(6, table);
      background-color: gray;
    }




