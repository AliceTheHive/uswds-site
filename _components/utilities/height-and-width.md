---
permalink: /utilities/height-and-width/
layout: styleguide
type: utility
title: Height and width
category: Utilities
lead: Set the dimensions of an item.
subnav:
- text: Height
  href: '#height'
- text: Width
  href: '#width'
- text: Maximum height
  href: '#maxh'
- text: Maximum width
  href: '#maxw'
- text: Minimum height
  href: '#minh'
- text: Minimum width
  href: '#minw'
- text: Aspect ratio
  href: '#aspect'
- text: Circle
  href: '#circle'
- text: Square
  href: '#square'
- text: Utility mixins
  href: '#utility-mixins'
- text: Advanced settings
  href: '#advanced-settings'

utilities:
- base:         height
  var:          height
  output:       true
  responsive:   false
  active:       false
  focus:        false
  hover:        false
  visited:      false
- base:         width
  var:          width
  output:       true
  responsive:   false
  active:       false
  focus:        false
  hover:        false
  visited:      false
- base:         maxh
  var:          max-height
  output:       true
  responsive:   false
  active:       false
  focus:        false
  hover:        false
  visited:      false
- base:         maxw
  var:          max-width
  output:       true
  responsive:   false
  active:       false
  focus:        false
  hover:        false
  visited:      false
- base:         minh
  var:          min-height
  output:       true
  responsive:   false
  active:       false
  focus:        false
  hover:        false
  visited:      false
- base:         minw
  var:          min-width
  output:       true,
  responsive:   false
  active:       false
  focus:        false
  hover:        false
  visited:      false
- base:         add-aspect
  var:          add-aspect
  output:       true
  responsive:   false
  active:       false
  focus:        false
  hover:        false
  visited:      false
- base:         circle
  var:          circle
  output:       true
  responsive:   false
  active:       false
  focus:        false
  hover:        false
  visited:      false
- base:         square
  var:          square
  output:       true
  responsive:   false
  active:       false
  focus:        false
  hover:        false
  visited:      false
---

{% assign height_values = site.data.uswds_tokens.special.auto_auto
  | concat: site.data.uswds_tokens.special.zero_zero
  | concat: site.data.uswds_tokens.spacing.positive.smaller
  | concat: site.data.uswds_tokens.spacing.positive.small
  | concat: site.data.uswds_tokens.spacing.positive.medium
  | concat: site.data.uswds_tokens.spacing.positive.large
  | concat: site.data.uswds_tokens.special.full_percent
  | concat: site.data.uswds_tokens.special.full_viewport_height
%}

{% assign width_values = site.data.uswds_tokens.special.auto_auto
  | concat: site.data.uswds_tokens.special.zero_zero
  | concat: site.data.uswds_tokens.spacing.positive.smaller
  | concat: site.data.uswds_tokens.spacing.positive.small
  | concat: site.data.uswds_tokens.spacing.positive.medium
  | concat: site.data.uswds_tokens.spacing.positive.large
  | concat: site.data.uswds_tokens.spacing.positive.larger
  | concat: site.data.uswds_tokens.spacing.positive.largest
  | concat: site.data.uswds_tokens.special.full_percent
%}

{% assign maxh_values = site.data.uswds_tokens.special.none_none
  | concat: site.data.uswds_tokens.spacing.positive.small
  | concat: site.data.uswds_tokens.spacing.positive.medium
  | concat: site.data.uswds_tokens.spacing.positive.large
  | concat: site.data.uswds_tokens.spacing.positive.larger
  | concat: site.data.uswds_tokens.special.full_viewport_height
%}

{% assign maxw_values = site.data.uswds_tokens.special.none_none
  | concat: site.data.uswds_tokens.spacing.positive.small
  | concat: site.data.uswds_tokens.spacing.positive.medium
  | concat: site.data.uswds_tokens.spacing.positive.large
  | concat: site.data.uswds_tokens.spacing.positive.larger
  | concat: site.data.uswds_tokens.spacing.positive.largest
  | concat: site.data.uswds_tokens.special.full_percent
%}

{% assign minh_values = site.data.uswds_tokens.special.none_none
  | concat: site.data.uswds_tokens.special.zero_zero
  | concat: site.data.uswds_tokens.spacing.positive.small
  | concat: site.data.uswds_tokens.spacing.positive.medium
  | concat: site.data.uswds_tokens.spacing.positive.large
  | concat: site.data.uswds_tokens.spacing.positive.larger
  | concat: site.data.uswds_tokens.special.full_percent
  | concat: site.data.uswds_tokens.special.full_viewport_height
%}

{% assign minw_values = site.data.uswds_tokens.special.none_none
  | concat: site.data.uswds_tokens.spacing.positive.small
  | concat: site.data.uswds_tokens.spacing.positive.medium
%}

{% assign circle_values = site.data.uswds_tokens.spacing.positive.smaller
  | concat: site.data.uswds_tokens.spacing.positive.small
  | concat: site.data.uswds_tokens.spacing.positive.medium
  | concat: site.data.uswds_tokens.spacing.positive.large
%}

{% assign square_values = site.data.uswds_tokens.spacing.positive.smaller
  | concat: site.data.uswds_tokens.spacing.positive.small
  | concat: site.data.uswds_tokens.spacing.positive.medium
  | concat: site.data.uswds_tokens.spacing.positive.large
%}

<div class="utilities-properties">
  <h3 class="utilities-property-title">CSS properties</h3>
  <div class="margin-top-1">
    <span class="token utilities-property">height</span>
    <span class="token utilities-property">max-height</span>
    <span class="token utilities-property">max-width</span>
    <span class="token utilities-property">min-height</span>
    <span class="token utilities-property">min-width</span>
    <span class="token utilities-property">width</span>
  </div>
</div>

<section class="utilities-section">
  <div class="grid-row utilities-section-title-bar">
    <h2 class="grid-col-auto utilities-section-title">Examples and usage</h2>
    <p class="grid-col-fill utilities-section-helper">Utilities, values, and variants may be activated and deactivated in <a href="#advanced-settings" class="text-ink text-no-wrap">advanced settings</a>.</p>
  </div>

  <section class="utility" id="height">
    <section class="utility-title-bar">
      <div class="grid-row">
        <div class="grid-col-fill">
          <h3 class="grid-col-auto utility-title">Height</h3>
          <p class="utility-property">CSS property: <span class="utility-property-code">height</span></p>
        </div>
        <ul class="grid-col-auto utility-scope">
          <li class="utility-scope-button-disabled">responsive</li>
          <li class="utility-scope-button-disabled">active</li>
          <li class="utility-scope-button-disabled">hover</li>
          <li class="utility-scope-button-disabled">focus</li>
          <li class="utility-scope-button-disabled">visited</li>
        </ul>
      </div>
    </section><!-- .utility-title-bar -->
    <section class="utility-examples">
      <div class="grid-row grid gap">
        {% for item in height_values %}
          <div class="grid-col-{% if forloop.last %}fill{% else %}2{% endif %} utility-example-container display-flex flex-column flex-justify-end">
              <div class="width-4 bg-secondary-light height-{{ item.token }}"></div>
              <div class="display-flex flex-column flex-align-start padding-top-2">
                <span class="utility-class">.height-{{ item.token }}</span>
                <span class="utility-value">{{ item.value }}</span>
              </div>
          </div>
        {% endfor %}
      </div>
    </section><!-- .utility-examples -->
  </section><!-- .utility#height -->

  <section class="utility" id="width">
    <section class="utility-title-bar">
      <div class="grid-row">
        <div class="grid-col-fill">
          <h3 class="grid-col-auto utility-title">Width</h3>
          <p class="utility-property">CSS property: <span class="utility-property-code">width</span></p>
        </div>
        <ul class="grid-col-auto utility-scope">
          <li class="utility-scope-button-disabled">responsive</li>
          <li class="utility-scope-button-disabled">active</li>
          <li class="utility-scope-button-disabled">hover</li>
          <li class="utility-scope-button-disabled">focus</li>
          <li class="utility-scope-button-disabled">visited</li>
        </ul>
      </div>
    </section><!-- .utility-title-bar -->
    <section class="utility-examples">
      <div class="grid-row grid gap">
        {% for item in width_values %}
          <div class="grid-col-12 utility-example-container-condensed grid-row flex-align-center {% if forloop.last %} border-0{% endif %}">
              <div class="grid-col-3 display-flex flex-column flex-align-start">
                <span class="utility-class">.width-{{ item.token }}</span>
                <span class="utility-value">{{ item.value }}</span>
              </div>
              <div class="grid-col-9 padding-left-2">
                <div class="height-4 bg-secondary-light width-{{ item.token }} maxw-full grid-col-auto"></div>
              </div>
          </div>
        {% endfor %}
      </div>
    </section><!-- .utility-examples -->
  </section><!-- .utility#width -->

  <section class="utility" id="maxh">
    <section class="utility-title-bar">
      <div class="grid-row">
        <div class="grid-col-fill">
          <h3 class="grid-col-auto utility-title">Maximum height</h3>
          <p class="utility-property">CSS property: <span class="utility-property-code">max-height</span></p>
        </div>
        <ul class="grid-col-auto utility-scope">
          <li class="utility-scope-button-disabled">responsive</li>
          <li class="utility-scope-button-disabled">active</li>
          <li class="utility-scope-button-disabled">hover</li>
          <li class="utility-scope-button-disabled">focus</li>
          <li class="utility-scope-button-disabled">visited</li>
        </ul>
      </div>
    </section><!-- .utility-title-bar -->
    <section class="utility-examples">
      {% for item in maxh_values %}
        <p class="utility-example-container-condensed {% if forloop.last %}border-0{% endif %}">
          <span class="utility-class">.maxh-{{ item.token }}</span>
          <span class="utility-value margin-left-2px">{{ item.value }}</span>
        </p>
      {% endfor %}
    </section><!-- .utility-examples -->
  </section><!-- .utility#maxh -->

  <section class="utility" id="maxw">
    <section class="utility-title-bar">
      <div class="grid-row">
        <div class="grid-col-fill">
          <h3 class="grid-col-auto utility-title">Maximum width</h3>
          <p class="utility-property">CSS property: <span class="utility-property-code">max-width</span></p>
        </div>
        <ul class="grid-col-auto utility-scope">
          <li class="utility-scope-button-disabled">responsive</li>
          <li class="utility-scope-button-disabled">active</li>
          <li class="utility-scope-button-disabled">hover</li>
          <li class="utility-scope-button-disabled">focus</li>
          <li class="utility-scope-button-disabled">visited</li>
        </ul>
      </div>
    </section><!-- .utility-title-bar -->
    <section class="utility-examples">
      {% for item in maxw_values %}
        <p class="utility-example-container-condensed {% if forloop.last %}border-0{% endif %}">
          <span class="utility-class">.maxw-{{ item.token }}</span>
          <span class="utility-value margin-left-2px">{{ item.value }}</span>
        </p>
      {% endfor %}
    </section><!-- .utility-examples -->
  </section><!-- .utility#maxw -->

  <section class="utility" id="minh">
    <section class="utility-title-bar">
      <div class="grid-row">
        <div class="grid-col-fill">
          <h3 class="grid-col-auto utility-title">Minimum height</h3>
          <p class="utility-property">CSS property: <span class="utility-property-code">min-height</span></p>
        </div>
        <ul class="grid-col-auto utility-scope">
          <li class="utility-scope-button-disabled">responsive</li>
          <li class="utility-scope-button-disabled">active</li>
          <li class="utility-scope-button-disabled">hover</li>
          <li class="utility-scope-button-disabled">focus</li>
          <li class="utility-scope-button-disabled">visited</li>
        </ul>
      </div>
    </section><!-- .utility-title-bar -->
    <section class="utility-examples">
      {% for item in minh_values %}
        <p class="utility-example-container-condensed {% if forloop.last %}border-0{% endif %}">
          <span class="utility-class">.minh-{{ item.token }}</span>
          <span class="utility-value margin-left-2px">{{ item.value }}</span>
        </p>
      {% endfor %}
    </section><!-- .utility-examples -->
  </section><!-- .utility#minh -->

  <section class="utility" id="minw">
    <section class="utility-title-bar">
      <div class="grid-row">
        <div class="grid-col-fill">
          <h3 class="grid-col-auto utility-title">Minimum width</h3>
          <p class="utility-property">CSS property: <span class="utility-property-code">min-width</span></p>
        </div>
        <ul class="grid-col-auto utility-scope">
          <li class="utility-scope-button-disabled">responsive</li>
          <li class="utility-scope-button-disabled">active</li>
          <li class="utility-scope-button-disabled">hover</li>
          <li class="utility-scope-button-disabled">focus</li>
          <li class="utility-scope-button-disabled">visited</li>
        </ul>
      </div>
    </section><!-- .utility-title-bar -->
    <section class="utility-examples">
      {% for item in minw_values %}
        <p class="utility-example-container-condensed {% if forloop.last %}border-0{% endif %}">
          <span class="utility-class">.minw-{{ item.token }}</span>
          <span class="utility-value margin-left-2px">{{ item.value }}</span>
        </p>
      {% endfor %}
    </section><!-- .utility-examples -->
  </section><!-- .utility#minw -->

  <section class="utility" id="aspect">
    <section class="utility-title-bar">
      <div class="grid-row">
        <div class="grid-col-fill">
          <h3 class="grid-col-auto utility-title">Aspect ratio</h3>
        </div>
        <ul class="grid-col-auto utility-scope">
          <li class="utility-scope-button-disabled">responsive</li>
          <li class="utility-scope-button-disabled">active</li>
          <li class="utility-scope-button-disabled">hover</li>
          <li class="utility-scope-button-disabled">focus</li>
          <li class="utility-scope-button-disabled">visited</li>
        </ul>
      </div>
    </section><!-- .utility-title-bar -->
    <section class="utility-examples">
      <div class="grid-row grid-gap">
        <div class="grid-col utility-example-container-condensed display-flex flex-column flex-justify">
          <div class="width-full add-aspect-9x16 bg-secondary-light"></div>
          <div class="display-flex flex-column flex-align-start margin-top-2">
            <span class="utility-class">.add-aspect-9x16</span>
          </div>
        </div>
        <div class="grid-col utility-example-container-condensed display-flex flex-column flex-justify">
          <div class="width-full add-aspect-1x1 bg-secondary-light"></div>
          <div class="display-flex flex-column flex-align-start margin-top-2">
            <span class="utility-class">.add-aspect-1x1</span>
          </div>
        </div>
        <div class="grid-col utility-example-container-condensed display-flex flex-column flex-justify">
          <div class="width-full add-aspect-4x3 bg-secondary-light"></div>
          <div class="display-flex flex-column flex-align-start margin-top-2">
            <span class="utility-class">.add-aspect-4x3</span>
          </div>
        </div>
        <div class="grid-col utility-example-container-condensed display-flex flex-column flex-justify">
          <div class="width-full add-aspect-16x9 bg-secondary-light"></div>
          <div class="display-flex flex-column flex-align-start margin-top-2">
            <span class="utility-class">.add-aspect-16x9</span>
          </div>
        </div>
        <div class="grid-col utility-example-container-condensed display-flex flex-column flex-justify">
          <div class="width-full add-aspect-2x1 bg-secondary-light"></div>
          <div class="display-flex flex-column flex-align-start margin-top-2">
            <span class="utility-class">.add-aspect-2x1</span>
          </div>
        </div>
      </div>
    </section><!-- .utility-examples -->
  </section><!-- .utility#aspect -->

  <section class="utility" id="circle">
    <section class="utility-title-bar">
      <div class="grid-row">
        <div class="grid-col-fill">
          <h3 class="grid-col-auto utility-title">Circle</h3>
        </div>
        <ul class="grid-col-auto utility-scope">
          <li class="utility-scope-button-disabled">responsive</li>
          <li class="utility-scope-button-disabled">active</li>
          <li class="utility-scope-button-disabled">hover</li>
          <li class="utility-scope-button-disabled">focus</li>
          <li class="utility-scope-button-disabled">visited</li>
        </ul>
      </div>
    </section><!-- .utility-title-bar -->
    <section class="utility-examples">
      <div class="grid-row grid-gap">
        {% for item in circle_values %}
          {% if forloop.index > 1 %}
            <div class="utility-example-container display-flex flex-column flex-justify{% if forloop.index > 13 and forloop.last == false %} grid-col-6{% elsif forloop.last %} grid-col-fill{% else %} grid-col-3{% endif %}">
              <div class="circle-{{ item.token }} bg-secondary-light"></div>
              <div class="display-flex flex-column flex-align-start margin-top-2">
                <span class="utility-class">.circle-{{ item.token }}</span>
                <span class="utility-value margin-left-2px">{{ item.value }}</span>
              </div>
            </div>
          {% endif %}
        {% endfor %}
      </div>
    </section><!-- .utility-examples -->
  </section><!-- .utility#circle -->

  <section class="utility" id="square">
    <section class="utility-title-bar">
      <div class="grid-row">
        <div class="grid-col-fill">
          <h3 class="grid-col-auto utility-title">Square</h3>
        </div>
        <ul class="grid-col-auto utility-scope">
          <li class="utility-scope-button-disabled">responsive</li>
          <li class="utility-scope-button-disabled">active</li>
          <li class="utility-scope-button-disabled">hover</li>
          <li class="utility-scope-button-disabled">focus</li>
          <li class="utility-scope-button-disabled">visited</li>
        </ul>
      </div>
    </section><!-- .utility-title-bar -->
    <section class="utility-examples">
      <div class="grid-row grid-gap">
        {% for item in square_values %}
          {% if forloop.index > 1 %}
            <div class="utility-example-container display-flex flex-column flex-justify{% if forloop.index > 13 and forloop.last == false %} grid-col-6{% elsif forloop.last %} grid-col-fill{% else %} grid-col-3{% endif %}">
              <div class="square-{{ item.token }} bg-secondary-light"></div>
              <div class="display-flex flex-column flex-align-start margin-top-2">
                <span class="utility-class">.square-{{ item.token }}</span>
                <span class="utility-value margin-left-2px">{{ item.value }}</span>
              </div>
            </div>
          {% endif %}
        {% endfor %}
      </div>
    </section><!-- .utility-examples -->
  </section><!-- .utility#square -->
</section>

<section class="utilities-section">
  <h2 class="utilities-section-title">Default output</h2>
  <div class="grid-row font-sans-1 text-bold border-bottom padding-bottom-05 margin-top-2 border-base-light">
    <div class="grid-col-4">Utility</div>
    <div class="grid-col-6">Output SCSS</div>
    <div class="grid-col-2">Default variable value</div>
  </div>
  <dl class="output-list">
    {% assign this_utility = 'height' %}
    {% assign this_property = 'height' %}
    {% for value in height_values %}
      <dt class="output-utility">.{{ this_utility }}-{{ value.token }}</dt>
      {% if value.scss %}
        <dd class="output-css">
          <span>{{ this_property }}: <span class="output-token">{{ value.scss }}</span>
          </span>
        </dd>
        <dd class="output-variable">{{ value.value }}</dd>
      {% else %}
        <dd class="output-css"><span>{{ this_property }}: {{ value.value }}</span></dd>
        <dd class="output-variable">—</dd>
      {% endif %}
    {% endfor %}

    {% assign this_utility = 'width' %}
    {% assign this_property = 'width' %}
    {% for value in width_values %}
      <dt class="output-utility">.{{ this_utility }}-{{ value.token }}</dt>
      {% if value.scss %}
        <dd class="output-css">
          <span>{{ this_property }}: <span class="output-token">{{ value.scss }}</span>
          </span>
        </dd>
        <dd class="output-variable">{{ value.value }}</dd>
      {% else %}
        <dd class="output-css"><span>{{ this_property }}: {{ value.value }}</span></dd>
        <dd class="output-variable">—</dd>
      {% endif %}
    {% endfor %}

    {% assign this_utility = 'maxh' %}
    {% assign this_property = 'max-height' %}
    {% for value in maxh_values %}
      <dt class="output-utility">.{{ this_utility }}-{{ value.token }}</dt>
      {% if value.scss %}
        <dd class="output-css">
          <span>{{ this_property }}: <span class="output-token">{{ value.scss }}</span>
          </span>
        </dd>
        <dd class="output-variable">{{ value.value }}</dd>
      {% else %}
        <dd class="output-css"><span>{{ this_property }}: {{ value.value }}</span></dd>
        <dd class="output-variable">—</dd>
      {% endif %}
    {% endfor %}

    {% assign this_utility = 'maxw' %}
    {% assign this_property = 'max-width' %}
    {% for value in maxw_values %}
      <dt class="output-utility">.{{ this_utility }}-{{ value.token }}</dt>
      {% if value.scss %}
        <dd class="output-css">
          <span>{{ this_property }}: <span class="output-token">{{ value.scss }}</span>
          </span>
        </dd>
        <dd class="output-variable">{{ value.value }}</dd>
      {% else %}
        <dd class="output-css"><span>{{ this_property }}: {{ value.value }}</span></dd>
        <dd class="output-variable">—</dd>
      {% endif %}
    {% endfor %}

    {% assign this_utility = 'minh' %}
    {% assign this_property = 'min-height' %}
    {% for value in minh_values %}
      <dt class="output-utility">.{{ this_utility }}-{{ value.token }}</dt>
      {% if value.scss %}
        <dd class="output-css">
          <span>{{ this_property }}: <span class="output-token">{{ value.scss }}</span>
          </span>
        </dd>
        <dd class="output-variable">{{ value.value }}</dd>
      {% else %}
        <dd class="output-css"><span>{{ this_property }}: {{ value.value }}</span></dd>
        <dd class="output-variable">—</dd>
      {% endif %}
    {% endfor %}

    {% assign this_utility = 'circle' %}
    {% assign this_property = 'height, width'
      | split: ', '
    %}
    {% assign this_rule = 'border-radius: 50%'
      | split: ', '
    %}
    {% for value in minw_values %}
      <dt class="output-utility">.{{ this_utility }}-{{ value.token }}</dt>
      {% if value.scss %}
        <dd class="output-css">
          <span>
            {% if this_property %}
              {% for property in this_property %}
              <span class="output-rule">{{ property }}: <span class="output-token">{{ value.scss }}</span></span>
              {% endfor %}
            {% endif %}
            {% if this_rule %}
              {% for rule in this_rule %}
              <span class="output-rule">{{ rule }}</span>
              {% endfor %}
            {% endif %}
          </span>
        </dd>
        <dd class="output-variable">{{ value.value }}</dd>
      {% else %}
        <dd class="output-css">
          <span>
            {% if this_property %}
              {% for property in this_property %}
              <span class="output-rule">{{ property }}: {{ value.value }}</span>
              {% endfor %}
            {% endif %}
            {% if this_rule %}
              {% for rule in this_rule %}
              <span class="output-rule">{{ rule }}</span>
              {% endfor %}
            {% endif %}
          </span>
        </dd>
        <dd class="output-variable">—</dd>
      {% endif %}
    {% endfor %}

    {% assign this_utility = 'square' %}
    {% assign this_property = 'height, width'
      | split: ', '
    %}
    {% assign this_rule = false %}
    {% for value in minw_values %}
      <dt class="output-utility">.{{ this_utility }}-{{ value.token }}</dt>
      {% if value.scss %}
        <dd class="output-css">
          <span>
            {% if this_property %}
              {% for property in this_property %}
              <span class="output-rule">{{ property }}: <span class="output-token">{{ value.scss }}</span></span>
              {% endfor %}
            {% endif %}
            {% if this_rule %}
              {% for rule in this_rule %}
              <span class="output-rule">{{ rule }}</span>
              {% endfor %}
            {% endif %}
          </span>
        </dd>
        <dd class="output-variable">{{ value.value }}</dd>
      {% else %}
        <dd class="output-css">
          <span>
            {% if this_property %}
              {% for property in this_property %}
              <span class="output-rule">{{ property }}: {{ value.value }}</span>
              {% endfor %}
            {% endif %}
            {% if this_rule %}
              {% for rule in this_rule %}
              <span class="output-rule">{{ rule }}</span>
              {% endfor %}
            {% endif %}
          </span>
        </dd>
        <dd class="output-variable">—</dd>
      {% endif %}
    {% endfor %}

  </dl>
</section>

<section id="utility-mixins" class="padding-top-4">
  <h2 class="margin-y-0">Utility mixins</h2>
  {% include utilities/utility-mixin-intro.html %}

  <div class="grid-row font-sans-3xs text-bold border-bottom border-base-light padding-bottom-05 margin-top-2 margin-top-3">
    <div class="grid-col-4">Utility</div>
    <div class="grid-col-4">Mixin</div>
    <div class="grid-col-4">Example</div>
  </div>
  <div class="grid-row font-mono-2xs padding-y-1 border-bottom border-base-light">
    <div class="grid-col-4">.height-<code>unit</code></div>
    <div class="grid-col-4">u-height(<code>value</code>)</div>
    <div class="grid-col-4">
      <span class="display-block">u-height('card')</span>
    </div>
  </div>
  <div class="grid-row font-mono-2xs padding-y-1 border-bottom border-base-light">
    <div class="grid-col-4">.width-<code>unit</code></div>
    <div class="grid-col-4">u-width(<code>value</code>)</div>
    <div class="grid-col-4">
      <span class="display-block">u-width('auto')</span>
    </div>
  </div>
  <div class="grid-row font-mono-2xs padding-y-1 border-bottom border-base-light">
    <div class="grid-col-4">.maxh-<code>unit</code></div>
    <div class="grid-col-4">u-maxh(<code>value</code>)</div>
    <div class="grid-col-4">
      <span class="display-block">u-maxh('screen')</span>
    </div>
  </div>
  <div class="grid-row font-mono-2xs padding-y-1 border-bottom border-base-light">
    <div class="grid-col-4">.maxw-<code>unit</code></div>
    <div class="grid-col-4">u-maxw(<code>value</code>)</div>
    <div class="grid-col-4">
      <span class="display-block">u-maxw('card-lg')</span>
    </div>
  </div>
  <div class="grid-row font-mono-2xs padding-y-1 border-bottom border-base-light">
    <div class="grid-col-4">.minh-<code>unit</code></div>
    <div class="grid-col-4">u-minh(<code>value</code>)</div>
    <div class="grid-col-4">
      <span class="display-block">u-minh('screen')</span>
    </div>
  </div>
  <div class="grid-row font-mono-2xs padding-y-1 border-bottom border-base-light">
    <div class="grid-col-4">.minw-<code>unit</code></div>
    <div class="grid-col-4">u-minw(<code>value</code>)</div>
    <div class="grid-col-4">
      <span class="display-block">u-minw('auto')</span>
    </div>
  </div>
  <div class="grid-row font-mono-2xs padding-y-1 border-bottom border-base-light">
    <div class="grid-col-4">.add-aspect-<code>ratio</code></div>
    <div class="grid-col-4">add-aspect(<code>value</code>)</div>
    <div class="grid-col-4">
      <span class="display-block">add-aspect('16x9')</span>
    </div>
  </div>
  <div class="grid-row font-mono-2xs padding-y-1 border-bottom border-base-light">
    <div class="grid-col-4">.circle-<code>unit</code></div>
    <div class="grid-col-4">u-circle(<code>value</code>)</div>
    <div class="grid-col-4">
      <span class="display-block">u-circle('05')</span>
    </div>
  </div>
  <div class="grid-row font-mono-2xs padding-y-1 border-bottom border-base-light">
    <div class="grid-col-4">.square-<code>unit</code></div>
    <div class="grid-col-4">u-square(<code>value</code>)</div>
    <div class="grid-col-4">
      <span class="display-block">u-square(2)</span>
    </div>
  </div>

  {% include utilities/utility-mixin-using.html %}
</section>

<section id="advanced-settings" class="padding-top-4">
  <h2 class="margin-y-0">Advanced settings</h2>

  {% include utilities/responsive-variants.html %}

  {% include utilities/state-variants.html %}

  {% include utilities/output-control.html %}

  <section class="utilities-section margin-top-6">
    {% include utilities/values-intro.html %}

    <aside class="example border-left-05 border-secondary-light padding-left-105 margin-top-2">
      <h4 class="font-sans-2xs margin-top-0 margin-bottom-05">Example</h4>
<pre class="font-mono-xs margin-0 padding-0 bg-transparent">
$width-palettes: (
  $palette-spacing-uswds-large // note: no trailing comma
);
</pre>
    <h4 class="font-sans-2xs margin-top-2 margin-bottom-05">Output</h4>
<pre class=" font-mono-xs margin-0 padding-0 bg-transparent">
.width-card { width: 10rem; }
.width-card-lg { width: 15rem; }
.width-mobile { width: 20rem; }
</pre>
    </aside>

    {% include utilities/standard-palettes.html %}
    {% include utilities/spacing-palettes.html %}

  </section>
</section>