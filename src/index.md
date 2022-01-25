---
# Feel free to add content and custom Front Matter to this file.

layout: default
---

<div class="recipe-list grid sm:grid-cols-2 lg:grid-cols-3 2xl:grid-cols-4 gap-8">
    <% collections.recipes.resources.each do |recipe| %>
    <%= render "recipe_card", recipe: recipe %>    
  <% end %>
</div>
