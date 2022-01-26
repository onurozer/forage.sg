---
# Feel free to add content and custom Front Matter to this file.

layout: default
---

<% site.categories.keys.each do |category| %>
  <div class="p-6 mb-6">
  <h2 class="text-4xl mb-6 text-yellow-700"><%= category %></h2>
  <div class="recipe-list grid sm:grid-cols-2 lg:grid-cols-3 2xl:grid-cols-4 gap-8">
  <% site.categories[category].each do |recipe| %>  
    <%= render "recipe_card", recipe: recipe %>    
    <% end %>
  </div>
  </div>
<% end %>
