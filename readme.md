# Active route/path template helpers for [Iron.Router](https://github.com/eventedmind/iron-router)
[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/zimme/meteor-iron-router-active?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

I used [iron-router-active](https://github.com/XpressiveCode/iron-router-active)
as inspiration and did a coffeescript rewrite as it wasn't very active, pun
intended :P Also made a small functional change and also an API rewrite.

### Usage
```html
<nav>
  <ul>
    <li class="{{isActiveRoute regex='dashboard'}}">...</li>
    <li class="{{isActiveRoute regex='dashboard|index'}}">...</li>
    <li class="{{isActiveRoute regex='users' className='on'}}">...</li>
    <li class="{{isActivePath regex='products'}}">...</li>
    {{#if isActiveRoute regex='index'}}
      <li>...</li>
    {{/if}}
  </ul>
</nav>
```
