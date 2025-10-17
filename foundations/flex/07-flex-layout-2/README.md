# The Holy Grail of Layout

In this last flexbox exercise you're going to recreate an incredibly common website layout. It is so common that it is often called the [Holy Grail](https://www.google.com/search?q=holy+grail+layout&tbm=isch&sclient=img) layout... and with flexbox it is actually pretty easy to pull off.

As with the previous exercise, we've left a little more for you to do.

### Hints

- You will need to change the flex-direction to push the footer down.
- You will need to add some divs as containers to get things to line up correctly.
- `flex-wrap` will help get the cards aligned correctly.
- Make sure you define how much space the cards should take up, in order for `flex-wrap` to work as intended.

## Desired outcome

![desired outcome](./desired-outcome.png)

The number of cards lined up in that section will change based on the width of your screen, so don't stress about getting _exactly_ a 2x3 or 3x2 grid.

On a smaller screen it will look like this:

![smaller](./desired-outcome-smaller.png)

Note: The emojis may instead show up as one or several text symbols (e.g. &#9734;&#9794;) if you don't have an emoji-based font family installed on your operating system. This does not affect the exercise and can be ignored.

### Self Check

- The header text is size 32px and weight 900.
  Added to .header selector:
  font-size: 32px;
  font-weight: 900;

- The header text is vertically centered and 16px from the edge of the screen.
  Added to.header selector:
  display: flex;
  align-items: center;
  padding-left: 16px;

- The footer is pushed to the bottom of the screen (the footer may go _below_ the bottom of the screen if the content of the 'cards' section overflows and/or if your screen is shorter).

.content {
flex: 1;
display: flex;
}

- The footer text is centered horizontally and vertically.
  .footer {
  display: flex;
  justify-content: center;
  align-items: center;
  }

- The sidebar and cards take up all available space above the footer.
  .content {
  flex: 1;
  display: flex;
  }

- The sidebar is 300px wide (and it doesn't shrink).
  .sidebar {
  flex-shrink: 0;}

- The sidebar links are size 24px, are white, and do not have the underline text decoration.
  .sideLink {
  text-decoration: none;
  color: white;
  font-size: 24px;
  }

- The sidebar has 16px padding.
  padding: 16px;
- There is 48px padding around the 'cards' section.

- The cards are arranged horizontally, but wrap to multiple lines when they run out of room on the page.
