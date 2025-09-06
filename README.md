# Gradient Text Animation

A simple and visually striking text animation effect using CSS, featuring a multi-color gradient that continuously shifts across the text. Perfect for adding dynamic, eye-catching typography to your projects.

## Features

- **Dynamic Gradient**: The text features a gradient animation that shifts smoothly across multiple colors.
- **Customizable Font**: Easily modify the font style, size, and weight for your needs.
- **Cross-browser Support**: Uses standard CSS properties to ensure compatibility across modern browsers.
- **Infinite Animation**: The gradient shift runs indefinitely with a smooth transition.

## Installation

To use this text animation in your own project, simply follow the steps below:

1. **Clone this repository**:

    ```bash
    git clone https://github.com/yourusername/gradient-text-animation.git
    ```

2. **Add the HTML and CSS**:

    Include the following HTML structure in your webpage:

    ```html
    <div class="text">Your Text Here</div>
    ```

    And add the accompanying CSS to your `style.css` or `<style>` tag:

    ```css
    *{
        padding: 0%;
        margin: 0%;
    }
    html,body{
        display: grid;
        height: 100%;
        place-items: center;
        background: #000;
    }
    .text{
        font-size: 110px;
        font-weight: 800;
        text-transform: uppercase;
        
        background: linear-gradient(135deg, #3f15e6, #ca1963, #ee3c3c, #5335cf);
        background-size: 400%;
        -webkit-background-clip: text;

        -webkit-text-fill-color: transparent;

        animation: animate 10s linear infinite;
    }
    @keyframes animate {
        100%{
            background-position: 400%;
        }
    }
    ```

3. **Customize the Text**: Replace the text inside the `<div class="text">Your Text Here</div>` with whatever you like.

## Customization

- **Font Size**: Adjust the `font-size` property in the `.text` class.
- **Animation Speed**: Modify the `10s` value in the `animation` property to speed up or slow down the gradient shift.
- **Gradient Colors**: Change the colors in the `background: linear-gradient()` to any color values you prefer.

## Browser Support

- Chrome
- Firefox
- Safari
- Edge

Ensure your browser is up to date to avoid any compatibility issues.

Enjoy the animated text effect! 🎨✨
