# jquery-active-link


```html
<!DOCTYPE html>
<html>
<head>
  <!-- JQuery reference -->
  <script src="https://code.jquery.com/jquery-3.6.0.js" integrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk=" crossorigin="anonymous"></script>
  
  <!-- Bootstrap css reference -->
  <link 
    rel="stylesheet" 
    href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" 
    integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" 
    crossorigin="anonymous">
    
    <!-- Bootstrap js reference -->
  <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
</head>

<body>
  
  <!-- Bootstrap nav -->
  <nav class="p-3 container navbar navbar-expand-lg navbar-light">
    <a class="navbar-brand" style="font-weight: bold;" href="#">
      Home
    </a>
    <button class="navbar-toggler" type="button" data-toggle="collapse"
      data-target="#navbarNav" aria-controls="navbarNav"
      aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <div class="navbar-nav mr-auto">
        <div class="nav-item">
          <a class="navbar-brand nav-link" 
          target="_blank"
          href="https://www.amazon.com/dp/B0C1NXJFPQ?tag=breakwindo-20">
          	#link1
          </a>
        </div>
        <div class="nav-item">
          <a class="navbar-brand nav-link" target="_blank"
          href="https://facestyling.click/">
          	#link2
          </a>
        </div>
      </div>
    </div>
  </nav>
  
  <script>  
   $(document).ready(function () {
     //change an active link dynamically
     $(".navbar-nav a").on("click", function(){
       $(".navbar-nav").find(".active").removeClass("active");
       $(this).parent().addClass("active");
     });  
   });
  </script>
  
</body>
</html>
```
