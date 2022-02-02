---
layout: default
---

<% collections.posts.resources.each do |post| %>
<a href="<%=post.relative_url%>"><%= post.data.title %></a><br />
<% end %>
