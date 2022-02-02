---
layout: default
---

<% collections.posts.resources.each do |post| %>
<a href="<%=post.relative_url%>"><%= post.data.title %></a>

<span class="<%= post.data.ingredients.nil? ? 'text-red-500' : 'text-green-500' %>">ingredients</span>
<span class="<%= post.data.servings.nil? ? 'text-red-500' : 'text-green-500' %>">servings</span>
<span class="<%= post.data.duration.nil? ? 'text-red-500' : 'text-green-500' %>">duration</span>

  <br />
<% end %>
