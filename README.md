# XSS-Cheat-Sheet

#Reflected XSS

Case 1: When inserted untrusted data into HTML element content
  <%
  string uinput = request.getParameter("input");
  %>
  <div><%= uninput %></div>
  
Case 2: When inserted untrusted data into HTML common attribute
  <%
  string uinput = request.getParameter("input");
  %>
  <div attr='<%= uninput %>'></div>
  
Case 3: When inserted untrusted data into JavaScript data value.
  <%
  string uinput = request.getParameter("input");
  %>
  <script>var a='<%= uninput %>';</script>
  

  
