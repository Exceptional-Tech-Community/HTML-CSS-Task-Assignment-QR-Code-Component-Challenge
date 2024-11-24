### HTML & CSS Task Assignment: QR Code Component Challenge  

The task involves creating a simple and responsive QR code card design using HTML and CSS. Below are the steps to complete the assignment: 

![png (8)](https://github.com/user-attachments/assets/b3012f61-9a46-4527-865d-0d980904d49a)
---

#### **1. Setting Up the HTML**  
Edit the `index.html` file by following these steps:  

1. **Main Structure**:  
   - Add a main container (`div.container`) to center all content.  

2. **Card Design**:  
   - Inside the container, create a `div.card` for the QR code card.  
   - Add a child `div.card-image` to hold the QR code image.  
   - Place an image (`img`) with the QR code inside `div.card-image`. Use an appropriate `src` and `alt`.  

3. **Content Section**:  
   - Create a `div.card-content` for the text content of the card.  
   - Add an `h1` for the title (e.g., *"Connect. Learn. Grow your skills by building projects"*).  
   - Add a `p` for the description (e.g., *"Scan the QR code to follow us and stay updated with the latest in tech."*).  

**HTML Code Example**:
```html
<body>
  <div class="container">
    <div class="card">
      <div class="card-image">
        <img src="images/ETC-QR-code-2.png" alt="QR code image" />
      </div>
      <div class="card-content">
        <h1>
          Connect. Learn. Grow your<br />
          skills by building projects
        </h1>
        <p>
          Scan the QR code to follow us and stay updated with the latest in tech.
        </p>
      </div>
    </div>
  </div>
</body>
```

---

#### **2. Setting Up the CSS**  
Create a `styles.css` file and follow these steps for styling:  

1. **Global Styles**:  
   - Import the `Outfit` font from Google Fonts.  
   - Apply a CSS reset using the `*` selector.  
   - Set the `font-family` to "Outfit" and a light blue background (`hsl(212, 45%, 89%)`) for the `body`.  

**CSS Code**:
```css
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@100..900&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Outfit", sans-serif;
  background-color: hsl(212, 45%, 89%);
}
```

2. **Container Styling**:  
   - Set the container height to `100vh`.  
   - Use `display: flex` with `justify-content: space-evenly` and `align-items: center` to center content vertically and horizontally.  
   - Set `flex-direction: column` to stack child elements.  

**CSS Code**:
```css
.container {
  height: 100vh;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  flex-direction: column;
}
```

3. **Card Styling**:  
   - Set the card width to `300px` and add padding of `15px`.  
   - Apply a white background (`hsl(0, 0%, 100%)`), rounded corners (`border-radius: 15px`), and a subtle shadow.  

**CSS Code**:
```css
.card {
  width: 300px;
  padding: 15px;
  background-color: hsl(0, 0%, 100%);
  border-radius: 15px;
  box-shadow: 0px 19px 13px rgba(0, 0, 0, 0.1);
}
```

4. **QR Code Image**:  
   - Restrict the image width to `100%`.  
   - Add padding to the image container and set a dark background for contrast.  

**CSS Code**:
```css
.card-image {
  width: 269px;
  height: 269px;
  border-radius: 15px;
  overflow: hidden;
  padding: 45px;
  background: #000006;
}

.card-image img {
  width: 100%;
  border-radius: 10px;
}
```

5. **Text Content**:  
   - Center-align text in the `card-content` section.  
   - Style the `h1` and `p` elements with appropriate font sizes, weights, and colors.  

**CSS Code**:
```css
.card-content {
  text-align: center;
}

.card-content h1 {
  color: hsl(218, 44%, 22%);
  font-size: 18px;
  font-weight: 700;
  margin-top: 15px;
}

.card-content p {
  color: hsl(216, 15%, 48%);
  font-size: 15px;
  font-weight: 400;
  margin-top: 15px;
  margin-bottom: 15px;
}
```

---

### **3. Task Completion**  
By following the steps above, you can create a responsive and minimal QR code card component. This challenge is a great way to practice:
- Semantic HTML structure.
- CSS Flexbox for layout.
- Clean and reusable CSS rules.  

Use this opportunity to refine your design and layout skills!
