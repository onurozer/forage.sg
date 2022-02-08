---
# Feel free to add content and custom Front Matter to this file.

layout: default
---

<% site.categories.keys.each do |category| %>

  <div class="px-6 mb-6">
  <h2 class="text-4xl mb-6 text-center"><a href="#<%=category%>"></a><%= category.capitalize %></h2>
  <div class="recipe-list grid md:grid-cols-2 xl:grid-cols-3 gap-6">
  <% site.categories[category].each do |recipe| %>
    <%= render "recipe_card", recipe: recipe %>
    <% end %>
  </div>
  </div>
<% end %>
