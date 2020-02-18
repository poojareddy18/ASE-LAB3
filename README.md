# ASE-LAB3
NUTRITION FACTS 
<DOCTYPE html!>
<html>
<head>
<h2> LOGIN PAGE </h2>
<style>
body
{
  background-image:url("https://st3.depositphotos.com/1558912/19061/i/1600/depositphotos_190618686-stock-photo-italian-food-background-on-white.jpg");
  background-color:lightblue;
}
h2{
  text-align:center;
  }
div{
  text-align:center;
  }
//div1{
   text-align:center;
}
//div2{
   text-align:center;
}
</style>

<form>
<div>
 <label for="email"><b>EMAIL:</b></label>
<input type="email" placeholder="ENTER EMAIL" id="EMAIL"><br> <br>

   <label for="psw"><b>PASSWORD:</b></label>
<input type="text" placeholder="ENTER PASSWORD" id="PASSWORD"><br> <br>

<input type="button" value="login" onclick="location.href='Foodcal1.html';">
<br>
 <label>
        <input type="checkbox" checked="checked" name="remember"> Remember me
 <br>
<br>
      </label>
DON'T HAVE AN ACCOUNT?


<a href="register.html">  REGISTER </a>
<br>
<br>
 <button type="button" onclick="document.getElementById('id01').style.display='none'" class="cancelbtn">Cancel</button> 


</div>
</form>
</head>
</html>
/* login page
 <DOCTYPE html!>
<html>
<head>
<h2> LOGIN PAGE </h2>
<style>
body
{
  background-image:url("https://st3.depositphotos.com/1558912/19061/i/1600/depositphotos_190618686-stock-photo-italian-food-background-on-white.jpg");
  background-color:lightblue;
}
h2{
  text-align:center;
  }
div{
  text-align:center;
  }
//div1{
   text-align:center;
}
//div2{
   text-align:center;
}
</style>
<form>
<div>



   <label for="email"><b>EMAIL:</b></label>
<input type="email" placeholder="ENTER EMAIL" id="EMAIL"><br> <br>

   <label for="psw"><b>PASSWORD:</b></label>
<input type="text" placeholder="ENTER PASSWORD" id="PASSWORD"><br> <br>

<input type="submit" value="login" text-align="center">
<br>
 <label>
        <input type="checkbox" checked="checked" name="remember"> Remember me
      </label>
<br>
<br>
DON'T HAVE AN ACCOUNT?
<input type="submit" value="Register" text-align="center">
</div>
</form>
</head>
</html>
register page

<DOCTYPE html!>
<html>
<head>
<h2> REGISTER PAGE </h2>
<style>
body
{
  background-image:url("https://st3.depositphotos.com/1558912/19061/i/1600/depositphotos_190618686-stock-photo-italian-food-background-on-white.jpg");
  background-color:lightblue;
}
h2{
  text-align:center;
  }
div{
  text-align:center;
  }
//div1{
   text-align:center;
}
//div2{
   text-align:center;
}
</style>
<form>
<div>
LAST NAME:
<input type="text" id=" "><br> <br>
FIRST NAME:
<input type="text" id="FIRST NAME"><br> <br>
EMAIL:
<input type="email" id="EMAIL"><br> <br>
PASSWORD:
<input type="text" id="PASSWORD"><br> <br>
CONFIRM PASSWORD:
<input type="text" id="CONFIRM PASSWORD"><br> <br>
<input type="submit" value="sign-up" text-align="center">

<br>
 <label>
        <input type="checkbox" checked="checked" name="remember"> Remember me
        <br>
        <br>
      </label>
<a href="ase-lab3.html"> click here for login</a>
<br>
<br>

</div>
</form>
</head>
</html>
*/
final output
<DOCTYPE html!>
<html>
<head>
<h2> LOGIN PAGE </h2>
<style>
body
{
  background-image:url("https://st3.depositphotos.com/1558912/19061/i/1600/depositphotos_190618686-stock-photo-italian-food-background-on-white.jpg");
  background-color:lightblue;
}
h2{
  text-align:center;
  }
div{
  text-align:center;
  }
//div1{
   text-align:center;
}
//div2{
   text-align:center;
}
</style>

<form>
<div>
 <label for="email"><b>EMAIL:</b></label>
<input type="email" placeholder="ENTER EMAIL" id="EMAIL"><br> <br>

   <label for="psw"><b>PASSWORD:</b></label>
<input type="text" placeholder="ENTER PASSWORD" id="PASSWORD"><br> <br>

<input type="button" value="login" onclick="location.href='Foodcal1.html';">
<br>
 <label>
        <input type="checkbox" checked="checked" name="remember"> Remember me
 <br>
<br>
      </label>
DON'T HAVE AN ACCOUNT?


<a href="register.html">  REGISTER </a>
<br>
<br>
 <button type="button" onclick="document.getElementById('id01').style.display='none'" class="cancelbtn">Cancel</button> 


</div>
</form>
</head>
</html> 

<!DOCTYPE html>
<html>

  <head>
     <meta charset="UTF-8">
     <title>FOOD</title>
     <h1>NUTRITION FACTS</h1>

     <style>
      body {
      background-image:url("https://previews.123rf.com/images/romastudio/romastudio1603/romastudio160300219/54088690-organic-food-background-studio-photo-of-different-fruits-and-vegetables-on-white-wooden-table-high-r.jpg");
      //background-color:lightblue;
       }
      h1 {
      color: black;
      text-align: center;
      }
      p {
       text-align: center;
       font-size: 1.25em;
        }
      div {
       text-align: center;
       font-size: 1.25em;
       padding: 50px;
       }
     </style>
     
     <script src="https://code.responsivevoice.org/responsivevoice.js?key=Ky7lOIxX"></script>
 


     <script>
     var food;
     var api= 'https://api.nutritionix.com/v1_1/search/';
     var apikey = '?results=0:1&fields=*&appId=9bc675e1&appKey=5868e025ea66d80d6898353b1eb36aaf';
     var appId = '?results=0:1&fields=*&appId=9bc675e1';
     
     function Foodcal() 
     {
  // Send request
     var Item = document.getElementById("Item").value;
     responsiveVoice.speak('Nutrition values of'+Item);
     console.log(Item);
     var url = api + Item + apikey;
   //loadJSON(url, gotData);
   //console.log(gotData);
 
     var request = new XMLHttpRequest()

  // Open a new connection, using the GET request on the URL endpoint

     request.open('GET',url , true)
     request.onload = function()
     {
  // Begin accessing JSON data here
     console.log(this.response);
     var data = JSON.parse(this.response);
     console.log(data);

     my_div.innerHTML = my_div.innerHTML +"<br>Water: <input type='text' id='Water'>"
         my_div.innerHTML = my_div.innerHTML +"<br>calories: <input type='text' id='calories'>"
         my_div.innerHTML = my_div.innerHTML +"<br>sugars: <input type='text' id='sugars'>"
         my_div.innerHTML = my_div.innerHTML +"<br>cholesterol: <input type='text' id='cholesterol'>"
         my_div.innerHTML = my_div.innerHTML +"<br>protein: <input type='text' id='protein'>"
       my_div.innerHTML = my_div.innerHTML +"<br>total fat: <input type='text' id='fat'>"


 
         document.getElementById("Water").value=data.hits[0].fields.nf_water_grams;
         document.getElementById("calories").value=data.hits[0].fields.nf_calories;
         document.getElementById("sugars").value=data.hits[0].fields.nf_sugars;
         document.getElementById("cholesterol").value=data.hits[0].fields.nf_cholesterol;
         document.getElementById("protein").value=data.hits[0].fields.nf_protein;
       document.getElementById("fat").value=data.hits[0].fields.nf_total_fat;
       
     }
request.send();
      }

     </script>
     
  </head>
  <body>
     <p>
     item: <input type="text" id="Item" name="Item">
     <br>
     <button id="submit" onclick="Foodcal()">submit</button>
     <br>
     <div id="my_div"></div>
     </p>
   
  </body>
</html>

     



