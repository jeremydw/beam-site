---
layout: default
body_class: body--index

logos:
- title: APEX
  image_url: /images/logo_apex.png
  url: "#TODO"
- title: Flink
  image_url: /images/logo_flink.png
  url: "#TODO"
- title: Spark
  image_url: /images/logo_spark.png
  url: "#TODO"
- title: Google Cloud Dataflow
  image_url: /images/logo_google_cloud.png
  url: "#TODO"

pillars:
- title: Unified
  body: Use a single programming model for both batch and streaming use cases.
- title: Portable
  body: Execute pipelines on multiple execution environments.
- title: Extensible
  body: Write and share new SDKs, IO connectors, and transformation libraries.

cards:
- quote: "Lorem ipsum dolor sit amit. Qaz qux."
  name: Person 1
- quote: "Lorem ipsum dolor sit amit. Qaz qux."
  name: Person 2
- quote: "Lorem ipsum dolor sit amit. Qaz qux."
  name: Person 3
---
<div class="hero section">
  <div class="hero__cols">
    <div class="hero__cols__col">
      <div class="hero__cols__col__content">
        <div class="hero__title">
          Apache Beam: An advanced unified programming model
        </div>
        <div class="hero__subtitle">
          Implement batch and streaming data processing jobs that run on any execution engine.
        </div>
        <div class="hero__ctas">
          <a class="button button--primary" href="/get-started/beam-overview/">Learn more</a>
          <a class="button" href="/get-started/quickstart-java/">Quickstart</a>
        </div>
      </div>
    </div>
    <div class="hero__cols__col">
      <div class="hero__blog">
        <div class="hero__blog__title">
          The latest from the blog
        </div>
        <div class="hero__blog__cards">
          {% for post in site.posts limit:3 %}
          <a class="hero__blog__cards__card" href="{{ post.url | prepend: site.baseurl }}">
            <div class="hero__blog__cards__card__title">{{post.title}}</div>
            <div class="hero__blog__cards__card__date">{{ post.date | date: "%b %-d, %Y" }}</div>
          </a>
          {% endfor %}
        </div>
      </div>
    </div>
  </div>
</div>

<div class="pillars section">
  <div class="pillars__title">
    All about beam
  </div>
  <div class="pillars__cols">
    {% for pillar in page.pillars %}
    <div class="pillars__cols__col">
      <div class="pillars__cols__col__title">
        {{pillar.title}}
      </div>
      <div class="pillars__cols__col__body">
        {{pillar.body}}
      </div>
    </div>
    {% endfor %}
  </div>
</div>

<div class="graphic section">
<div class="graphic__image">
<img src="/images/beam_architecture.png">
</div>
</div>

<div class="logos section">
  <div class="logos__title">
    Works with
  </div>
  <div class="logos__logos">
    {% for logo in page.logos %}
    <div class="logos__logos__logo">
      <a href="{{logo.url}}"><img src="{{logo.image_url}}"></a>
    </div>
    {% endfor %}
  </div>
</div>

<div class="cards section section--wide">
  <div class="section__contained">
    <div class="cards__title">
      A collaborative effort
    </div>
    <div class="cards__cards">
      {% for card in page.cards %}
      <div class="cards__cards__card">
        <div class="cards__cards__card__body">
          {{card.quote}}
        </div>
        <div class="cards__cards__card__user">
          <div class="cards__cards__card__user__icon">
          </div>
          <div class="cards__cards__card__user__name">
            {{card.name}}
          </div>
        </div>
      </div>
      {% endfor %}
    </div>
    <div class="cards__body">
      Beam is an open source community and contributions are greatly appreciated!
      If you’d like to contribute, please see the <a href="/contribute/">Contribute</a> section.
    </div>
  </div>
</div>

<div class="ctas section">
  <div class="ctas__title">
    Get started
  </div>
  <div class="ctas__ctas">
  <a class="button button--primary" href="/get-started/beam-overview/">Learn more</a>
  <a class="button" href="/get-started/quickstart-java/">Quickstart</a>
  </div>
</div>
