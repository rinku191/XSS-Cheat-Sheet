# XSS-Cheat-Sheet

#Reflected XSS

Case 1: When inserted untrusted data into HTML element content<br>
  <%<br>
  string uinput = request.getParameter("input");<br>
  %><br>
  <div><%= uninput %></div><br>
  
Case 2: When inserted untrusted data into HTML common attribute<br>
  <%<br>
  string uinput = request.getParameter("input");<br>
  %><br>
  <div attr='<%= uninput %>'></div><br>
  
Case 3: When inserted untrusted data into JavaScript data value<br>
  <%<br>
  string uinput = request.getParameter("input");<br>
  %><br>
  <script>var a='<%= uninput %>';</script><br>
  

  
