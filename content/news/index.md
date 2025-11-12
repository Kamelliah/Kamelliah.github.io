---
# News Widget for Hugo Blox
widget: pages
headless: true

# This file represents a page section.
active: true

# Order that this section appears on the page.
weight: 60

title: Latest News
subtitle: ''

content:
  # Page type to display (e.g., post, event, publication)
  page_type: post
  # Choose how many pages you would like to display (0 = all pages)
  count: 6
  # Filter on criteria
  filters:
    author: ""
    category: "news"
    tag: ""
    exclude_featured: false
    exclude_future: false
    exclude_past: false
    publication_type: ""
  # Choose how many pages you would like to offset by
  offset: 0
  # Page order: descending (desc) or ascending (asc) date.
  order: desc

design:
  # Choose a view for the listings:
  #   1 = List
  #   2 = Compact
  #   3 = Card
  view: 3
  columns: '3'
---
