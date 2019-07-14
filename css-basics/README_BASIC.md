CSS is run by the browser

---

3 ways of adding css :

1. Inline CSS
2. CSS Selector
3. External CSS

---

Inline CSS:

- property: value ->
  property/decleartion : what you want to style.
  value : How you want to style.

- Adding the CSS directly on the element itslef.
- Not recommended way of doing. bcoz : Maintainability bcome difficult

---

CSS Selector

- In head section we are writing <style> </style> tag.
- Inside this style tag add the CSS Rules.
- Selector : is additional piece of information, which tell DOM to which element you want to assign the Styling for.
- Syntax :

  selector {
  property : value; // CSS Rule
  }

- Selector name can be -> Element name, id, class, universal, Attribute

---

External Style Sheet CSS

- Declaring all the styling in the external Style sheet file.
- Recommended approach, Separation of concern, Reusability, Browser no need to redownload for every new page.

---

- Default font family are present in the browser, Chrome > Settings > Search : Customize fonts >
  You will get different fonts preset.
- To use custome fonts: Search of Google Fonts. for ex:
  https://fonts.google.com/specimen/Barriecito?selection.family=Barriecito
  In your css file : add (import--) and the font-family assign the value of this google font which you have imported

---

- Selector name can be -> Element name, id, class, universal, Attribute
- Element : Selector name is html element/node name itself. Thus applying the styling to all the
  same element with that styling.
- Classes : Used to apply the styling for the elements within the same class. Think Student in the same class
  has common feature
