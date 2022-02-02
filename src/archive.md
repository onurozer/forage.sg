---
layout: default
---

<% collections.posts.resources.each do |post| %>
<a href="<%=post.relative_url%>"><%= post.data.title %></a> | i: <%= !post.data.ingredients.nil? %> | s: <%= !post.data.servings.nil? %> | d: <%= !post.data.duration.nil? %> <br />
<% end %>
