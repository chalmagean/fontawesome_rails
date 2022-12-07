Here's how to user fontawesome in your Rails 7 app with Importmaps.

1. Pin fontawesome

Add the following to your `config/importmap.rb` file.

```ruby
pin "@fortawesome/fontawesome-free",
  to: "https://ga.jspm.io/npm:@fortawesome/fontawesome-free@6.1.1/js/all.js"
```

2. Import it in your `app/javascript/application.js` file.

```javascript
import "@fortawesome/fontawesome-free";
```

3. Use it in your views.

```erb
<%= link_to "/" do %>
  <i class="fa-sharp fa-solid fa-house"></i>
  Click me
<% end %>
```
