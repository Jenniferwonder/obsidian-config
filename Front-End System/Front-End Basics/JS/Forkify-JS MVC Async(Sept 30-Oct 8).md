---
title: Forkify-JS MVC Async(Sept 30-Oct 8)
tags: null
status: null
started: null
due: null
aliases: null
---
## Project Overview
A single-page web app
#### TIME

| **Start Time** | Sept 30 |
| --- | --- |
| **Due Time** | Oct 8>  |
| **Total Time Spent** | 9 Days>  |
| **New Issues Added** | 

- ...
 |
#### TOOL
- **NPM& Node.js **
   - package.json > package-lock.json
   - install dev-dependencies
- **Parcel/ Webpack**
   - live-server
#### CODE
- HTML
- SASS/ CSS
- JS
## CSS/SCSS Layout (Layout/ Style/ Animation)
#### Typography
- Heading-1: Food-name (section-main-heading)
- Heading-2: Bold, colored and capitalized (section-sub-heading)
- Heading-3: capitalized (button info)
- Text (content info)
#### Background
- Linear-gradient
#### Header
- Favicon.png (an icon displayed in the header)
- Logo (an icon and a name with customized font)
- Search bar (Button (with a search icon))
   - search recipe from an API
   - heading-3: search (white)
- Buttons: 
   - heading-3: Add recipe (icon, black, bold)
      - Form popup
   - heading-3: Bookmarks (icon,  black, bold)
      - Bookmarked recipe preview
#### Sidebar
- Results preview list
- Page icons (show results in different pages)
   - display the search results 
- Footer
   - display copyright
#### Recipe section: 
- **Loading-icon** (displayed when loading)
- **Recipe data **from API (displayed after loading the required data from an API)
   - Main-photo
   - Heading-1: Food-name
   - Section-header
      - cooking time (time icon)
      - service (people icon)
      - user (user icon-round)
      - bookmark (bookmark icon-round with primary color)
   - Heading-2: Bold, colored and capitalized
      - Ingredients
         - 2 columns of lists (each with a tick icon)
      - How to cook
         - Button
            - heading-3: directions
## Folder Structure
### Root folder
- //.parcel-cache
- //dist
- //node_modules
- package.json
- package-lock.json
- ./src
### Src Folder
#### ASSETS: img
#### HTML: index.html
#### SASS: sass
- _base.scss
- _components.scss
- _header.scss
- _preview.scss
- _recipe.scss
- _searchResults.scss
- _upload.scss
- **main.scss**
#### JS: js (MVC Pattern)
- model.js
- controller.js
- helpers.js
- config.js
- ./views
   - View.js
   - recipeView.js
   - resultsView.js
   - searchView.js
   - previewView.js
   - paginationView.js
   - bookmarksView.js
   - addRecipeView.js
## JS Modules
- Render Spinner in HTML (Loading-icon)
- Show Recipe from API
   - Fetch Recipe data from API
   - Name and store recipe data
   - Render recipe in HTML
### Key Issues
