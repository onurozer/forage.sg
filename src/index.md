---
# Feel free to add content and custom Front Matter to this file.

layout: default
---

<main class="p-10">
  <div class="pb-6">
    <h1 class="text-2xl"><a href="/">Recipes</a></h1>
    <p> Everything you ever dreamt of.</p>
  </div>

<div class="recipe-list grid sm:grid-cols-2 lg:grid-cols-3 2xl:grid-cols-4 gap-8">
    <% collections.recipes.resources.each do |recipe| %>
    <%= render "recipe_card", recipe: recipe %>    
  <% end %>
</div>
</main>
