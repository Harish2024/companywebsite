# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Harish Electronic Private Limited
    </div></title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'img/title.jng' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
        harish Electronic Private Limited.
    </div>
    <div class="menu">
        <div class="menuitem"><a href="/home">Home</a></div> 
        <div class="menuitem"><a href="/products">Products</a></div> 
        <div class="menuitem"><a href="/people">People</a></div>
        <div class="menuitem"><a href="/contact">Contact Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2020 Dinesh Electronic Private Limited, Developed by Harisf G.
    </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/building2.jpeg" alt="Building">
    <div class="contenttext">
    Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c1.jpg" alt="product image">
            </div>
            <div class="itemname">4GB DDRA4 laptop memory</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c2.jpg"  alt="product image">
            </div>
            <div class="itemname">1TB Laptop HDD</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/harddrive.jpg"  alt="product image">
            </div>
            <div class="itemname">SEA SHELL SATA 2.5 inch SATA External hard drive Casing</div>
            <div class="itemprice">Price: Rs.379.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/homethrature.jpg" alt="product image">
            </div>
            <div class="itemname">Zebronics BT4440 RUCF 60 Watt Bluetooth Home Theatre</div>
            <div class="itemprice">Price: Rs.2999.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/usb.jpg" alt="product image">
            </div>
            <div class="itemname">Play Run USB Electric Dual Flameless Lighter Torch Rech</div>
            <div class="itemprice">Price: Rs.794.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/m1.jpg" alt="product image">
            </div>
            <div class="itemname">Boult Audio Thunder Bluetooth Headset</div>
            <div class="itemprice">Price: Rs.1299.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/m2.jpg" alt="product image">
            </div>
            <div class="itemname">Gigabyte NVIDIA GeForce GT 710 2 GB DDR3 Graphics Card</div>
            <div class="itemprice">Price: Rs.3299.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/m3.jpg" alt="product image">
            </div>
            <div class="itemname">CSD-255-21 Combo Box Analog Watch </div>
            <div class="itemprice">Price: Rs.330.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/m4.jpg" alt="product image">
            </div>
            <div class="itemname">Casio FX-991ES Plus-2nd Edition Scientific Scientific </div>
            <div class="itemprice">Price: Rs.1087.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/m5.jpg" alt="product image">
            </div>
            <div class="itemname">Regatech PA5108U-1BRS, PA5109U-1BRS, PA5110U 6 Cell Lap</div>
            <div class="itemprice">Price: Rs.2756.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/m8.jpg" alt="product image">
            </div>
            <div class="itemname">Canon EOS 3000D DSLR Camera Single Kit with 18-55 lens (16 GB Memory Card & Carry Case)  (Black)</div>
            <div class="itemprice">Price: Rs.27835.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/m6.jpg" alt="product image">
            </div>
            <div class="itemname">15 inch Expandable Laptop Backpack</div>
            <div class="itemprice">Price: Rs.450.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/m7.jpg" alt="product image">
            </div>
            <div class="itemname">Pitambara USB Type C to 3 Port USB 3.0 and Lan RJ45 </div>
            <div class="itemprice">Price: Rs.1249.00 </div>
        </div>
    </div>
    </div>
{% endblock  %}
```
### people.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1>Our Peoples</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/a1.jpg" alt="product image">
            </div>
            <div class="itemname">Saran V</div>
            <div class="itemprice">Company Head </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/a2.jpg"  alt="product image">
            </div>
            <div class="itemname">chetan v</div>
            <div class="itemprice">Company account Executive Agency </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/a3.jpg"  alt="product image">
            </div>
            <div class="itemname">Dinesh k</div>
            <div class="itemprice">Company Account Manager </div>
        </div>
        
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/a4.jpg" alt="product image">
            </div>
            <div class="itemname">aari D</div>
            <div class="itemprice">Ajency Development Manager </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/a5.jpg" alt="product image">
            </div>
            <div class="itemname">Harikrishnan V</div>
            <div class="itemprice">Bussiness Development Manager </div>
        </div>
  
      
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/a6.jpg" alt="product image">
            </div>
            <div class="itemname">suresh S </div>
            <div class="itemprice">Program Manager </div>
        </div>
    </div>
    </div>
{% endblock  %}

```
### contact.html
```

{% extends "website/base.html" %}

{% block content %}
    <div class="homecont">    
    <h1>Contact Us</h1>
    
    <div class="contenttext">
    <p style="font-size:30px">email : harishelectroniclimited@gmail.com</p>
    <p style="font-size:30px">ph.no : +91 44456 77789    +91 88856 00075</p>
    
    </div>
    </div>
{% endblock  %}

```


## OUTPUT:
![output](./static/img/o1.png)

![output](./static/img/o2.png)
![output](./static/img/o4.png)
![output](./static/img/o5.png)

## CODE VALIDATION REPORT:
![output](./static/img/r1.png)

![output](./static/img/r2.png)
![output](./static/img/r5.png)
![output](./static/img/r6.png)

## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://harish.student.saveetha.in:8000/. HTML code is validated.