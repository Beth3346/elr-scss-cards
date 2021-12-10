# Cards

[![npm version](http://img.shields.io/npm/v/elr-scss-cards.svg)](https://www.npmjs.org/package/elr-scss-cards)
[![CI](https://github.com/Beth3346/elr-scss-cards/actions/workflows/node.js.yml/badge.svg)](https://github.com/Beth3346/elr-scss-cards/actions/workflows/node.js.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![npm](https://img.shields.io/npm/dm/elr-scss-cards.svg?style=flat)](https://www.npmjs.com/package/elr-scss-cards)
[![last commit](https://img.shields.io/github/last-commit/Beth3346/elr-scss-cards.svg)](https://github.com/Beth3346/elr-scss-cards)
[![Netlify Status](https://api.netlify.com/api/v1/badges/f890da8d-40c3-4c09-aac2-9cc79c75ffea/deploy-status)](https://app.netlify.com/sites/elr-cards/deploys)

a library of sass mixins

[View Demo](https://elr-cards.netlify.app/)

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
npm install elr-scss-cards
```

or

```sh
yarn add elr-scss-cards
```

## Implementation

### Scss

```scss
.card {
  @include elr-card;
}
```

```scss
.card-border {
  @include elr-card(
    $config: (
      border-color: $light-gray,
      shadow: none,
    )
  );
}
```

```scss
.card-rounded {
  @include elr-card(
    $config: (
      border-color: $light-gray,
      shadow: none,
      border-radius: $base-fontsize * 0.5,
    )
  );
}
```

```scss
.card-centered {
  @include elr-card-centered;
}
```

### HTML

```html
<div class="card">
  <div class="card-inner">
    <div class="card-header">
      <div class="header-content">
        <h2 class="card-title">Title of Card</h2>
        <h3 class="card-subtitle">This is a subtitle for this card</h3>
      </div>
    </div>
    <div class="card-body">
      <div class="card-content">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem
          aspernatur cum culpa quasi deleniti. Accusamus nobis quo labore iure
          amet non, nihil corporis?
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem
          aspernatur cum culpa quasi deleniti. Accusamus nobis quo labore iure
          amet non, nihil corporis?
        </p>
      </div>
    </div>
    <div class="card-footer">
      <div class="card-actions">
        <a class="elr-button elr-button-primary">Button Link</a>
        <a class="elr-button elr-button-danger">Button Link</a>
      </div>
    </div>
  </div>
</div>
```

## License

SEE LICENSE IN LICENSE.md
