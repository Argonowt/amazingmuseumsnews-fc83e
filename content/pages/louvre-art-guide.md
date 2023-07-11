---
'0':
  type: string
  name: layout
  label: Layout
  const: PageLayout
  hidden: true
'1':
  type: string
  name: metaTitle
  label: Title meta tag (overrides title)
  description: >-
    By default, the <title> tag for this page is determined by the title field
    (in the Content group). You can override the tag value here.
  default: null
  group: seo
'2':
  type: string
  name: metaDescription
  label: Description meta tag
  description: >-
    The description tag is used by search engines and for social sharing. By
    default, the tag is not set.
  default: null
  group: seo
'3':
  type: boolean
  name: addTitleSuffix
  label: Add title suffix
  description: >-
    If enabled, the title suffix defined in the site configuration is appended
    to the title tag of this page.
  default: true
  group: seo
'4':
  type: image
  name: socialImage
  label: Image for social sharing
  description: >-
    Set the image used when sharing this page on social networks (e.g. Facebook,
    Twitter). If not set, the default social image defined in the site
    configuration is used.
  default: null
  group: seo
'5':
  type: list
  name: metaTags
  label: Additional meta tags
  description: >-
    To add or override any meta tag for this page, add entries to this list.
    Entries defined here take precedence over any other defaults.
  group: seo
  items:
    type: model
    models:
      - MetaTag
'6':
  type: string
  name: title
  label: Title
  default: This is a new page
  required: true
'7':
  type: list
  name: sections
  label: Sections
  items:
    type: model
    models:
      - ContactSection
      - CtaSection
      - DividerSection
      - FeatureHighlightSection
      - FeaturedItemsSection
      - FeaturedPeopleSection
      - FeaturedPostsSection
      - HeroSection
      - MediaGallerySection
      - QuoteSection
      - RecentPostsSection
      - TestimonialsSection
      - TextSection
  default:
    - type: HeroSection
      elementId: homepage-hero-1
      colors: colors-d
      title: This Is A Big Hero Headline
      text: >-
        Aenean eros ipsum, interdum quis dignissim non, sollicitudin vitae nisl.
        Aenean vel aliquet elit, at blandit ipsum. Sed eleifend felis sit amet
        erat molestie, hendrerit malesuada justo ultrices. Nunc volutpat at erat
        itae interdum. Ut nec massa eget lorem blandit condimentum et at risus.
      actions:
        - type: Button
          label: Get Started
          url: /
          style: primary
          elementId: hero-main-button
        - type: Button
          label: Learn More
          url: /
          style: secondary
      media:
        type: ImageBlock
        url: /images/hero.webp
        altText: Image alt text
      styles:
        self:
          height: auto
          width: wide
          margin:
            - mt-0
            - mb-0
            - ml-0
            - mr-0
          padding:
            - pt-12
            - pb-12
            - pl-4
            - pr-4
          alignItems: center
          justifyContent: center
          flexDirection: row
        title:
          textAlign: left
        subtitle:
          fontWeight: 400
          fontStyle: normal
          textAlign: left
        text:
          textAlign: left
        actions:
          justifyContent: flex-start
layout: PageLayout
metaTitle: null
metaDescription: null
addTitleSuffix: true
socialImage: null
metaTags: []
title: The Louvre - Art Guide
sections:
  - type: HeroSection
    colors: colors-d
    elementId: ''
    backgroundSize: full
    title: The Louvre Art Guide
    subtitle: Carlos Javier Taranilla de la Varga
    text: |+
      *   Collection: Amazing Museums

      *   Size: 14 x 21 cm

      *   Pages: 345

      *   Format: Paperback with color illustrations

      *   Edition: 1st edition

      *   Release date: November 2022

      *   ISBN: 9788418943454

      *   ISBN POD: 9788418943461

      *   ISBN ebook: 9788418943478

      *   RRP: 19,95€.

    actions:
      - type: Button
        label: Buy the paperback book
        showIcon: true
        icon: cart
        style: primary
        url: >-
          https://www.amazon.com/-/es/Carlos-Javier-Taranilla-Varga/dp/8418943459/
    media:
      type: ImageBlock
      url: /images/978-84-1894-342-3.png
      altText: Hero image
    backgroundImage: null
    styles:
      self:
        height: auto
        width: wide
        padding:
          - pt-36
          - pb-48
          - pl-4
          - pr-4
        alignItems: center
        justifyContent: center
        flexDirection: row-reverse
      title:
        textAlign: left
      subtitle:
        textAlign: left
      text:
        textAlign: left
      actions:
        justifyContent: flex-start
  - type: TextSection
    colors: colors-d
    variant: variant-a
    text: >
      <center><iframe width="560" height="315"
      src="https://www.youtube.com/embed/YHTncinyS70" title="YouTube video
      player" frameborder="0" allow="accelerometer; autoplay; clipboard-write;
      encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen></iframe></center>
    styles:
      self:
        height: auto
        width: narrow
        margin:
          - mb-12
        padding:
          - pt-0
          - pb-0
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      text:
        textAlign: left
  - type: TextSection
    colors: colors-d
    elementId: ''
    variant: variant-b
    title: The Louvre Art Guide
    subtitle: >-
      The essential artistic guide to discover and learn the essentials of the
      greatest works, artists and styles in the Louvre Museum.
    text: >
      Discover the immense art collection of the Louvre Museum, from Oriental,
      Egyptian, Greco-Roman and medieval antiquities to the great works of the
      Renaissance, Baroque, Neoclassicism and Romanticism. Painting, sculpture
      and decorative arts from all periods and civilizations. Works by great
      French masters such as Poussin and David, Flemish painters such as Rubens
      and Van Dyck, Dutch artists such as Rembrandt, Italian masters such as
      Leonardo da Vinci, Raphael, Michelangelo, Titian and Tintoretto, and
      Spanish artists such as El Greco, Zurbarán, Velázquez and Goya. An
      essential book to delve into the structure of the Louvre palace and its
      dependencies, learning in detail about 120 essential masterpieces among
      the more than 400,000 pieces contained in the most important museum in the
      world.
    styles:
      self:
        height: auto
        width: wide
        padding:
          - pt-24
          - pb-2
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      text:
        textAlign: left
  - type: TextSection
    colors: colors-d
    elementId: ''
    variant: variant-a
    text: |
      <center>![](/images/1689076016-removebg-preview.png)</center>
    styles:
      self:
        height: auto
        width: narrow
        padding:
          - pt-0
          - pb-0
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: center
      subtitle:
        textAlign: center
      text:
        textAlign: center
  - type: TextSection
    colors: colors-a
    elementId: ''
    variant: variant-a
    title: What makes this guide different from other Louvre guides?
    text: >+
      *   Learn about the history of one of the most important museums in the
      world: 120 essential masterpieces arranged by school, style and author. 


      *   Clear, complete and rigorous information on artists, works, periods
      and collections in general that the museum treasures in its headquarters. 


      *   Written in a didactic way both for the non-specialized reader and for
      students and the general public who wish to learn about the Louvre’s
      artistic treasures. 


      *   The accuracy of its exposition and the practical approach it provides,
      makes this book a useful work, both to prepare and to remember the visit
      to the museum. 


      *   Glossary of artistic terms necessary to understand the specialized
      concepts of the text and to establish relationships between the different
      stages of the history of art.

    styles:
      self:
        height: auto
        width: narrow
        padding:
          - pt-24
          - pb-24
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: center
      subtitle:
        textAlign: center
      text:
        textAlign: center
  - type: FeaturedItemsSection
    colors: colors-d
    elementId: ''
    title: Links of interest
    subtitle: ''
    items:
      - type: FeaturedItem
        text: >
          Download the first chapter and start discovering all that this museum
          has to offer.
        actions:
          - type: Button
            label: Download
            showIcon: true
            icon: arrowRight
            url: >-
              https://drive.google.com/file/d/1l9g36EHGJF-m8zCG9fgr3BdfRG1KD2fM/view?usp=sharing
            style: secondary
        styles:
          self:
            textAlign: left
        featuredImage:
          type: ImageBlock
          url: /images/1689000208-d3aa3593.png
          altText: altText of the image
          caption: Caption of the image
          elementId: ''
      - type: FeaturedItem
        text: |
          Buy the book on Amazon or AmazingMuseums.com
        actions:
          - type: Button
            label: Buy the book
            showIcon: true
            icon: arrowRight
            url: 'https://www.amazon.es/dp/8418943394/'
            style: secondary
        styles:
          self:
            textAlign: left
        featuredImage:
          type: ImageBlock
          url: /images/agas-removebg-preview.png
          altText: altText of the image
          caption: Caption of the image
          elementId: ''
      - type: FeaturedItem
        text: |
          Want to know more about the book? Download the product sheet.
        actions:
          - type: Button
            label: Download
            showIcon: true
            icon: arrowRight
            url: >-
              https://drive.google.com/file/d/1FHQTgSHr6PB1x0x5KTMidzaFYR_0BHF7/view?usp=sharing
            style: secondary
        styles:
          self:
            textAlign: left
        featuredImage:
          type: ImageBlock
          url: /images/1689076016-removebg-preview.png
          altText: altText of the image
          caption: Caption of the image
          elementId: ''
    actions: []
    columns: 3
    spacingX: 16
    spacingY: 16
    enableHover: false
    styles:
      self:
        height: auto
        width: wide
        padding:
          - pt-28
          - pb-36
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      actions:
        justifyContent: flex-start
---
