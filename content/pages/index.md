---
title: Home
layout: PageLayout
sections:
  - type: DividerSection
    colors: colors-d
    styles:
      self:
        width: wide
        padding:
          - pt-0
          - pb-6
          - pl-0
          - pr-0
        justifyContent: center
        borderWidth: 1
        borderStyle: solid
  - type: FeatureHighlightSection
    colors: colors-d
    elementId: ''
    backgroundSize: full
    title: The essential guides to discover and admire the best museums in the world
    subtitle: ''
    text: |
      Author and director of the book series: Carlos Taranilla
    actions:
      - type: Button
        label: Buy the books
        showIcon: true
        icon: arrowRight
        style: primary
        url: 'https://amazingmuseums.com'
    backgroundImage:
      type: ImageBlock
      url: /images/prado vector.png
      backgroundSize: cover
      backgroundPosition: center
      opacity: 100
    styles:
      self:
        height: auto
        width: wide
        padding:
          - pt-36
          - pb-72
          - pl-4
          - pr-4
        justifyContent: flex-start
      title:
        textAlign: left
      subtitle:
        textAlign: left
      text:
        textAlign: left
      actions:
        justifyContent: flex-start
  - type: FeaturedPostsSection
    colors: colors-d
    elementId: ''
    showDate: true
    showAuthor: false
    showExcerpt: true
    showReadMoreLink: true
    readMoreLinkLabel: Read more
    variant: variant-c
    actions:
      - type: Link
        label: Read all the articles
        altText: Read all the articles
        url: /blog
        showIcon: true
        icon: arrowRight
    styles:
      self:
        height: auto
        width: wide
        padding:
          - pt-24
          - pb-24
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      actions:
        justifyContent: flex-start
    title: 'Read the latest articles, curiosities and news'
    subtitle: ''
    posts:
      - content/pages/blog/post-five.md
      - content/pages/blog/post-four.md
      - content/pages/blog/post-three.md
      - content/pages/blog/post-two.md
      - content/pages/blog/post-one.md
  - type: QuoteSection
    colors: colors-d
    quote: |
      "Museums are places where time is transformed into space."
    name: Orhan Pamuk
    title: Nobel Prize in Literature in 2006
    styles:
      self:
        height: auto
        width: wide
        padding:
          - pt-28
          - pb-36
          - pr-4
          - pl-4
        justifyContent: center
      quote:
        textAlign: center
      name:
        textAlign: center
      title:
        textAlign: center
  - type: DividerSection
    colors: colors-d
    styles:
      self:
        width: wide
        padding:
          - pt-4
          - pb-4
          - pl-4
          - pr-4
        justifyContent: center
        borderWidth: 1
        borderStyle: solid
addTitleSuffix: true
metaTags: []
---
