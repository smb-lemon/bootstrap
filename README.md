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