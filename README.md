# Credit Card UI with Flip Animation

This project showcases a responsive and interactive credit card UI using HTML, CSS, and JavaScript. It features a card flip animation to display the front and back sides of a simulated credit card.

## Features
- **Card Flip Animation:** Users can view the front and back of the card using a smooth 3D flip effect.
- **Responsive Design:** Mobile-friendly layout with adaptive components.
- **Glassmorphism Effect:** Modern, frosted glass UI with glowing animations.
- **State Bank of India Branding:** Custom design with SBI branding and a MasterCard logo.

## Project Structure
```
├── index.html       # Main HTML structure
├── style.css        # Styling and animations
├── script.js        # JavaScript for interactive behavior
├── sbi.jpg          # Background image (State Bank of India theme)
```

## How It Works
1. **Front Side:** Displays the cardholder's name, card number (partially visible), and the card type.
2. **Back Side:** Displays additional card details such as the CVV, expiration date, and security chip.
3. **Flip Effect:** Clicking on "View Card Details" or "Hide Card Details" toggles the card flip using CSS animations.

## Installation & Usage
1. Clone the repository:
    ```bash
    git clone <repository-url>
    ```
2. Open the `index.html` file in a browser.
3. Ensure `style.css`, `script.js`, and `sbi.jpg` are in the same directory.

## Code Overview

### HTML (`index.html`)
- Structured using semantic HTML5.
- Card front and back are placed within a `#card-container`.
- Buttons trigger the flip animation via JavaScript.

### CSS (`style.css`)
- Implements a glassmorphic design with a glowing animation.
- Uses keyframe animations to animate the card border.
- Gradient text effects are applied using `-webkit-background-clip`.
- The flip effect uses `transform: rotateY()` with smooth transitions.

### JavaScript (`script.js`)
- Simple logic using event listeners to toggle the `flipped` class.
- Adds movement to the reflection effect using CSS transitions.

```javascript
flip = () => {
    document.getElementById('card').classList.toggle('flipped');
    document.querySelector('#front .reflection').classList.toggle('move');
    document.querySelector('#back .reflection').classList.toggle('move');
}
document.getElementById('show-btn').addEventListener('click', flip);
document.getElementById('hide-btn').addEventListener('click', flip);
```

## Credits
- **State Bank of India (SBI)**: Design inspired by SBI branding.
- **MasterCard**: Logo displayed for educational and UI purposes.
- **Author**: Syed Shafinali Syed Ashraf Ali

## License
This project is for educational purposes only. The design and branding are inspired by real-world entities but are not affiliated with or endorsed by them.

