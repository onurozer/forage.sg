---
# Feel free to add content and custom Front Matter to this file.

layout: default
---

<% site.categories.keys.each do |category| %>
<!-- Category -->
<div class="px-6 mb-12">
  <h2 class="text-2xl font-black mb-6 text-center  "><a id="<%=category%>"></a><%= category %></h2>
  <!-- Recipe List -->
  <div class="recipe-list grid md:grid-cols-2 xl:grid-cols-3 gap-9">
    <% site.categories[category].each do |recipe| %>
      <%= render "recipe_card", recipe: recipe %>
    <% end %>
  </div>
</div>
<% end %>
