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

- Different types of selector -> Element name, id, class, universal, Attribute

- Element : Selector name is html element/node name itself. Thus applying the styling to all the
  same element with that styling.
  html:
  <-h1 class="tilte"> Hello <-/h1>
  css:
  h1{
  color : red;
  }
- Classes : Used to apply the styling for the elements within the same class. Think Students in the same class
  has common feature (i.e- Common Styling Applied).
  Classes are best when we are reusing the Styling. Whereas, ID is best when we want to apply the style for
  a particular element only.

  ex -html:

  <-h1 class="tilte"> Hello <-/h1>
  <-h2 class="tilte"> World <-/h2>

  css :
  .title {
  color : red;
  }
  NOTE : naming convention of class and ID's name should be kebab-cases. Also css is case incensitive for ex-
  sectionTitile is same as sectiontitile in CSS class name thus you me result up in overidding the Styling.

- Universal : Applies the styling to all the elements of that html page. Thinks Students in the same college.
  css : \* {
  color : red;
  }
- ID's : Setting the styling to specific element by identifiying using unique identified i.e- id value, think
  applying a feature to specific student with his uid (Id card)
  ex - html :

  <-h1 id="main-tilte"> Hello <-/h1>

  css :
  #main-title {
  color : red;
  }

- Attribute : Set styling to all elements with attribute
  ex - html :
  <-button disabled> Click <-/button>
  css :
  [disabled] {
  color : red;
  }

---

- CSS Specifity: We know that multiple styling can be applied on the same element.Thus Specificity provides/tell order/priority of the styling which will be applied.
- CSS parse the rules from top to bottom approach.
- Open the chrome dev tools > Elements (tab) > Styles (below tab) > Note : the order of styles applied is showed from top to bottom ( for ex- first element.style{ } -> is inline style )
- CSS - Casading Style Sheets -> Casading means multiple styles/multipe css rules can be applied to same
  element.
- Specifity: Resolves conflicts arising from multiple rule
- order of specificity :
  1. !important (Highest specifity)
  2. Inline Style
  3. #ID selector
  4. .class, :pseudo-class and [attribute] selector
  5. Element/Tag Selector, Universal selector and ::pseudo-element selector (Lowest specifity)

https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity

---
