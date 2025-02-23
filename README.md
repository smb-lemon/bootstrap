# Bootstrap

[Bootstrap](https://getbootstrap.com/docs/5.3/getting-started/introduction/) is a powerful, feature-packed frontend toolkit 
which is used to build anything from prototype to production
in a short period of time.

### Benefits
- make development faster and easier
- good choice of pre-building component
- good browser compatibility

### CDN (Content Delivery Network)
 > CSS Link : `https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css `<br>
 JS Link : `https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js`

### Container

Containers are used to contain, padding and sometimes center the content
within them.

| Size         | Extra Small (<576px) | Small (≥576px) | Medium (≥768px) | Large (≥992px) | X-Large (≥1200px) | XX-Large (≥1400px) |
|-------------|---------------------|---------------|----------------|---------------|------------------|------------------|
| `.container`     | 100% | 540px | 720px | 960px | 1140px | 1320px |
| `.container-sm`  | 100% | 540px | 720px | 960px | 1140px | 1320px |
| `.container-md`  | 100% | 100% | 720px | 960px | 1140px | 1320px |
| `.container-lg`  | 100% | 100% | 100% | 960px | 1140px | 1320px |
| `.container-xl`  | 100% | 100% | 100% | 100% | 1140px | 1320px |
| `.container-xxl` | 100% | 100% | 100% | 100% | 100% | 1320px |
| `.container-fluid` | 100% | 100% | 100% | 100% | 100% | 100% |

### Button
Examples:
```css
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-warning">Warning</button>
```

### Button Group

Group a series of buttons together on a single line or stack 
them in a vertical column.
```html
<div class="btn-group" role="group" aria-label="Basic outlined example">
  <button type="button" class="btn btn-outline-primary">Left</button>
  <button type="button" class="btn btn-outline-primary">Middle</button>
  <button type="button" class="btn btn-outline-primary">Right</button>
</div>
```

### Bedges

Bedges are used to add how many notification or message etc are there.
 Examples:

<button type="button" class="btn btn-primary">
    Notifications <span class="badge text-bg-secondary">+6</span>
    </button> <br>
    
```html
    <button type="button" class="btn btn-primary">
    Notifications <span class="badge text-bg-secondary">4</span>
    </button>
```

<button type="button" class="btn btn-primary position-relative">
  Inbox
  <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
    99+
    <span class="visually-hidden">unread messages</span>
  </span>
</button>

```html
<button type="button" class="btn btn-primary position-relative">
  Inbox
  <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
    99+
    <span class="visually-hidden">unread messages</span>
  </span>
</button>
```

### Alerts

Provide contextual feedback messages for typical user actions with the handful of available and flexible alert messages

```html
<div class="alert alert-info" role="alert">
  A simple info alert—check it out!
</div>
<div class="alert alert-light" role="alert">
  A simple light alert—check it out!
</div>
<div class="alert alert-dark" role="alert">
  A simple dark alert—check it out!
</div>
```
### Navbar

Documentation and examples for Bootstrap’s powerful, responsive navigation header, the navbar. Includes support for branding, navigation, and more, including support for our collapse plugin.

- navbar-brand for your company, product, or project name.
- navbar-nav for a full-height and lightweight navigation (including support for dropdowns).
- navbar-toggler for use with our collapse plugin and other navigation toggling behaviors.
Flex and spacing utilities for any form controls and actions.
- navbar-text for adding vertically centered strings of text.
- collapse.navbar-collapse for grouping and hiding navbar contents by a parent breakpoint.
- Add an optional .navbar-scroll to set a max-height and scroll expanded navbar content.

Example: 
```html
<nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Features</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Pricing</a>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" aria-disabled="true">Disabled</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
```

### Card

A card is a flexible and extensible content container. It includes options for headers and footers, a wide variety of content, contextual background colors, and powerful display options. If you’re familiar with Bootstrap 3, cards replace our old panels, wells, and thumbnails. Similar functionality to those components is available as modifier classes for cards. <br>
Example: 
```html
<div class="card" style="width: 18rem;">
  <img src="..." class="card-img-top" alt="...">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
  <ul class="list-group list-group-flush">
    <li class="list-group-item">An item</li>
    <li class="list-group-item">A second item</li>
    <li class="list-group-item">A third item</li>
  </ul>
  <div class="card-body">
    <a href="#" class="card-link">Card link</a>
    <a href="#" class="card-link">Another link</a>
  </div>
</div>
```