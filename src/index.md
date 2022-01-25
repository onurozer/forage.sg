---
# Feel free to add content and custom Front Matter to this file.

layout: default
---

<ul>
  <% collections.recipes.resources.each do |recipe| %>
    <li>
      <a href="<%= recipe.relative_url %>"><%= recipe.data.title %></a>
    </li>
  <% end %>
</ul>
