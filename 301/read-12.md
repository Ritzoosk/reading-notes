# EJS Partials
- reuseable static elements
  - like nav bar
  - or header
  - stored in partial folder
  - <%- include('folder/file')%>
- very EASY!

> Note: The <%- %> tags allow us to output the unescaped content onto the page (notice the -). This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’, etc…

