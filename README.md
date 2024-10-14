# Thinkfulbnb - Vacation Rental Website

Thinkfulbnb is a vacation rental website that allows people to rent out their homes to people who are seeking short-term accommodations in that locale. Thinkfulbnb hosts rent out different kinds of properties, including single rooms, apartments, and unique living spaces such as yachts, houseboats, yurts, tiny houses, and even renovated medieval castles.
This project implements the Thinkfulbnb landing page using **HTML** and **CSS**, following a mobile-first design approach and using **flexbox** for layout management.


## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Project Setup](#project-setup)
- [Form Inputs](#form-inputs)
- [Responsive Design](#responsive-design)
  - [Mobile View](#mobile-view)
  - [Desktop View](#desktop-view)
- [Media Queries](#media-queries)
- [Technologies Used](#technologies-used)
- [Thinkfulbnb views](thinkful-views)
  - [Mobile Views](#mobile-views)
  - [Desktop Views](#desktop-views)
  - [Existing files](#existing-files)
  - [Setup](#setup)
  - [Tasks](#tasks)
      - [Navigation](#navigation)
      - [Media query](#media-query)
      - [Responsive images](#responsive-images)
      - [Vertical content alignment](#vertical-content-alignment)
      - [HTML form](#html-form)
        
## Project Overview

The goal of this project is to build a fully responsive landing page for the Thinkfulbnb vacation rental service. The project includes a **search form**, **responsive navigation**, and dynamically aligned images and text sections. The design adjusts based on the screen size, offering a great user experience on both mobile and desktop.

## Features

- Responsive navigation menu with anchor links to specific sections of the page.
- A vacation rental search form with appropriate input types.
- Layout designed using **flexbox**.
- **Mobile-first** approach to ensure the best user experience on smaller devices.
- Responsive images that adjust to the size of their containers.
- Vertical and horizontal alignment of text and images in different sections.
- Use of **media queries** to adapt the layout for larger screens (desktop view).

## Project Setup

To run this project locally, follow these steps:

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/your-username/thinkfulbnb.git
   cd thinkfulbnb
   ```
2. Open the project in VSCode or another code editor, and use Live Server to preview the webpage:
   ```bash
   code .
   ```
3. Run the Live Server extension in VSCode to launch the index.html file in your browser and see the page in action.

## Form Inputs
The search form is located in the "Find the perfect vacation rental" section. It contains the following input fields:

  + Location: Text input with a placeholder of "Search destination".
  + Arrive: Date input for the arrival date.
  + Depart: Date input for the departure date.
  + Type: Dropdown list with the following options:
      + Apartment
      + Barn
      + Castle
      + Houseboat
      + Tiny House
      + Yacht
      + Yurt
  + Search: A button to submit the form.
These fields are styled using custom CSS to align labels and inputs and create a polished, user-friendly form.

## Responsive Design
### Mobile View

In the mobile-first design:

  + The navigation logo and menu links are stacked vertically.
  + Images and content are stacked on top of each other in the **About**, **Ideas**, and **Host** sections.
  + The form inputs and labels are aligned properly for mobile usability.

### Desktop View
When the screen width exceeds 768px, the layout changes to adapt to larger screens:

  + The logo and navigation links are spaced horizontally.
  + The search form inputs and the button are aligned horizontally.
  + The **About** section content is aligned horizontally, with text being twice as wide as the images.
  + The **Ideas** section images are displayed in a 2x2 grid.
  + The **Host** section content is aligned horizontally, with text and images side-by-side.
## Media Queries
Media queries are used to implement the desktop layout. Specifically, a media query for screens wider than **768px** ensures:

  + The navigation menu becomes horizontal with adequate spacing between the logo and the links.
  + The search form fields and button are aligned in a row.
  + Text and images in the **About** and **Host** sections align horizontally.
  ```css
  /* Media query for screens wider than 768px */
  @media screen and (min-width: 768px) {
    /* Desktop styles here */
  }
  ```
## Technologies Used
  + **HTML**: For structuring the web page content.
  + **CSS**: For styling the page, including layout, typography, and responsive design.
  + **Flexbox**: Used to build flexible and responsive layouts.
  + **Media Queries**: Used to adapt the layout for different screen sizes.
  + **VSCode Live Server**: For live reloading during development.
    

## Thinkfulbnb views

The UX designer provided the following user interface mockups:

### Mobile views

![](images/Thinkfulbnb-mobile.png)

### Desktop views

![](images/Thinkfulbnb-desktop.png)

### Existing files

| File         | Description                                                             |
| ------------ | ----------------------------------------------------------------------- |
| `images/`    | A folder containing all the images used for the design.                 |
| `index.html` | The starter HTML file. The solution is added to this file. |
| `style.css`  | The starter css file. The solution is added to this file.  |

### Setup

Use VSCode Live Server to launch the `index.html` page in browser.

### Tasks

Use a mobile-first development approach. 

**should** use flexbox, and **not** floats, to achieve the desired layouts. The `.group`, `.item`, and `.item-double` classes are provided in the CSS file for your convenience, but it is not necessary to use them.

**NOT** expected to match the designs pixel by pixel, as long as the required layout is satisfied.

Edit the `index.html` and `style.css` as needed to achieve the following requirements:

#### Navigation

- The logo should stack on top of the menu links, which are aligned horizontally, as follows:

![Navigation mobile](./images/navigation-mobile.png)

- **Single-page navigation**: Modify the navigation links so that clicking on each link will take the user to the corresponding sections on the page, as follows:

| Link clicked | Take the user to the section with `id` of |
| ------------ | ----------------------------------------- |
| `Stay`       | `id="stay"`                               |
| `About`      | `id="about"`                              |
| `Ideas`      | `id="ideas"`                              |
| `Host`       | `id="host"`                               |

#### HTML form

- In the "Find your perfect vacation rental" section, create a form that contains the following input fields with the specified types:

  - `Location`: `text` input type, with a placeholder value of "Search destination"
  - `Arrive`: `date` input type
  - `Depart`: `date` input type
  - `Type`: a dropdown list with the following options:
    - Apartment
    - Barn
    - Castle
    - Houseboat
    - Tiny House
    - Yacht
    - Yurt
  - a `"Search"` button 

-  Add CSS to the form so that
  - the labels (i.e., "Location", "Arrive", "Depart", "Type") and their corresponding form fields are aligned towards the opposite ends of each row

Your final form design should look as follows:

![Search form mobile](./images/search-form-mobile.png)

#### Vertical content alignment

- The content in the remainder of the sections (i.e., "About", "Ideas", "Want to become a Thinkfulbnb Host?"), including any text and images, should stack on top of each other. Refer to the mobile design shared above.

#### Responsive images


- Write CSS for all images so that the images will match whatever container width they are placed within, and changing the container sizes will update the image sizes appropriately.

#### Media query: Desktop view

Once the mobile design is looking good, adapt the design for the desktop view.

- In `style.css`, create a media query for screens that are wider than `768px`.

Within the media query, write CSS to create the following designs for desktop:

- The logo and the navigation menu links should be spaced apart from each other, like this:

![Navigation desktop](./images/navigation-desktop.png)

- The search form input fields and the button should be horizontally aligned, like this:

![Search form desktop](./images/search-form-desktop.png)

- The items in the "About" section should be horizontally aligned. The paragraph content should be vertically centered and always be about twice as wide as each image item, like this:

![About desktop](./images/about-desktop.png)

- The "Ideas" images should be displayed in a 2 by 2 grid (see the desktop design shared above).

- The items in the "Want to Become a Thinkful Host?" section should be horizontally aligned. The paragraph content should be vertically centered and be as wide as each image item, like this:

![Host desktop](./images/host-desktop.png)

## Contributing
Contributions are welcome! If you have suggestions or improvements, feel free to submit a pull request.

