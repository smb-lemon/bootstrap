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

### Grid Layout

Use powerful mobile-first flexbox grid to build layouts of all shapes and sizes thanks to a twelve column system, six default responsive tiers, Sass variables and mixins, and dozens of predefined classes.

**How it works** <br> 
Breaking it down, here’s how the grid system comes together:

Our grid supports six responsive breakpoints. Breakpoints are based on min-width media queries, meaning they affect that breakpoint and all those above it (e.g., .col-sm-4 applies to sm, md, lg, xl, and xxl). This means you can control container and column sizing and behavior by each breakpoint.

Containers center and horizontally pad your content. Use .container for a responsive pixel width, .container-fluid for width: 100% across all viewports and devices, or a responsive container (e.g., .container-md) for a combination of fluid and pixel widths.

Rows are wrappers for columns. Each column has horizontal padding (called a gutter) for controlling the space between them. This padding is then counteracted on the rows with negative margins to ensure the content in your columns is visually aligned down the left side. Rows also support modifier classes to uniformly apply column sizing and gutter classes to change the spacing of your content.

Columns are incredibly flexible. There are 12 template columns available per row, allowing you to create different combinations of elements that span any number of columns. Column classes indicate the number of template columns to span (e.g., col-4 spans four). widths are set in percentages so you always have the same relative sizing.

Gutters are also responsive and customizable. Gutter classes are available across all breakpoints, with all the same sizes as our margin and padding spacing. Change horizontal gutters with .gx-* classes, vertical gutters with .gy-*, or all gutters with .g-* classes. .g-0 is also available to remove gutters.

Sass variables, maps, and mixins power the grid. If you don’t want to use the predefined grid classes in Bootstrap, you can use our grid’s source Sass to create your own with more semantic markup. We also include some CSS custom properties to consume these Sass variables for even greater flexibility for you.

**Grid options**<br> 
Bootstrap’s grid system can adapt across all six default breakpoints, and any breakpoints you customize. The six default grid tiers are as follows:

- Extra small (xs)
- Small (sm)
- Medium (md)
- Large (lg)
- Extra large (xl)
- Extra extra large (xxl)

| Size        | Breakpoint   | Container Max-Width | Class Prefix  |
|------------|-------------|--------------------|--------------|
| **xs**     | `<576px`    | None (auto)       | `.col-`      |
| **sm**     | `≥576px`    | 540px             | `.col-sm-`   |
| **md**     | `≥768px`    | 720px             | `.col-md-`   |
| **lg**     | `≥992px`    | 960px             | `.col-lg-`   |
| **xl**     | `≥1200px`   | 1140px            | `.col-xl-`   |
| **xxl**    | `≥1400px`   | 1320px            | `.col-xxl-`  |

### Additional Information:
- **# of columns:** 12  
- **Gutter width:** 1.5rem (0.75rem on left and right)  
- **Custom gutters:** Yes  
- **Nestable:** Yes  
- **Column ordering:** Yes  

Example: 
```html
<div class="container text-center">
  <div class="row">
    <div class="col">
      1 of 2
    </div>
    <div class="col">
      2 of 2
    </div>
  </div>
  <div class="row">
    <div class="col">
      1 of 3
    </div>
    <div class="col">
      2 of 3
    </div>
    <div class="col">
      3 of 3
    </div>
  </div>
</div>
```
### Grid Alignment
using flexbox alignment utilities to vertically and horizontally align columns.<br>
Examples:
```html
<div class="container text-center">
  <div class="row align-items-center">
    <div class="col">
      One of three columns
    </div>
    <div class="col">
      One of three columns
    </div>
    <div class="col">
      One of three columns
    </div>
  </div>
</div>
``` 
### Form Control
Give textual form controls like <input>s and <textarea>s an upgrade with custom styles, sizing, focus states, and more.

Example:
```html
<input class="form-control form-control-lg" type="text" placeholder=".form-control-lg" aria-label=".form-control-lg example">
<input class="form-control" type="text" placeholder="Default input" aria-label="default input example">
<input class="form-control form-control-sm" type="text" placeholder=".form-control-sm" aria-label=".form-control-sm example">
```