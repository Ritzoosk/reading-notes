# EJS

- EJS is a templating language
- similar to mustache in that it help to make templates for rendering to the page
- it allows you to insert data into specified locations in your template.
- no need to write code to generate your own HTML.
- it is not a "client-side" system.

- you can write conditionals right into the .ejs template
- ejs brackets = <%'stuff'%>
- You can insert partial data to generate elements
- layout are not native to express but EJS still works with them with the right library.
  - <%- layout %>

# questions
- deLimiters?
- CLI?
- static catching of intermediate JS and templates?

# Install
- npm install ejs

# Tags
"<% 'Scriptlet' tag, for control-flow, no output
<%_ ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it
<%= Outputs the value into the template (HTML escaped)
<%- Outputs the unescaped value into the template
<%# Comment tag, no execution, no output
<%% Outputs a literal '<%'
%> Plain ending tag
-%> Trim-mode ('newline slurp') tag, trims following newline
_%> ‘Whitespace Slurping’ ending tag, removes all whitespace after it"