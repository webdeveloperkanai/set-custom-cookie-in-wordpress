# Set custom cookie in wordpress
So many time I have tried but I could not add any coockie or session to store some temprary data. Finally I tried the javascript codes to store the cookie and it worked for me. 

You can also try this code to store any cookie in WordPress or php or HTML sites also.


<code>
     
     <script>
              function setCookie(name,value,days) {
                  if (days) {
                      var date = new Date();
                      date.setTime(date.getTime()+(days*24*60*60*1000));
                      var expires = "; expires="+date.toGMTString();
                  }
                  else var expires = "";
                  document.cookie = name+"="+value+expires+"; path=/";
              }
              setCookie('mypid','5',1);
    </script>
     
  </code>
  
  ## For more updates visit our website https://devsecit.com/
  ### Kanai Shil - DEV SEC IT Pvt. Ltd.
