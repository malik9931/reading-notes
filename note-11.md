![](https://miro.medium.com/max/720/1*DG4VA127mu4Fx2TrRIzskw.jpeg)

# EJS Templating

**EJS** simply stands for **Embedded JavaScript templates**, and we can use it both **server-side** or **client-side**. At this story, we’ll focus on the server-side.

## Basic Syntax(Tags):
1. `<%` 'Scriptlet' tag, for control-flow, no output
2. `<%=` Outputs the value into the template (HTML escaped)
3. `<%-` Outputs the unescaped value into the template

Example:

```
<% if (message) { %>
  <h2><%= message.name %></h2>
<% } %>
```


Install express and ejs:
```
npm i express --save
npm i ejs --save 
```
