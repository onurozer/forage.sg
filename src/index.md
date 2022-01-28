---
# Feel free to add content and custom Front Matter to this file.

layout: default
---

<% site.tags.keys.each do |tag| %>

  <div class="p-6 mb-6">
  <h2 class="text-4xl mb-6 text-center"><%= tag %></h2>
  <div class="recipe-list grid md:grid-cols-2 xl:grid-cols-3 gap-6">
  <% site.tags[tag].each do |recipe| %>
    <%= render "recipe_card", recipe: recipe %>
    <% end %>
  </div>
  </div>
<% end %>
