# ButterPop.js 🧈

![ButterPop.js](https://img.shields.io/badge/ButterPop.js-lightblue?style=flat&logo=javascript)

Welcome to **ButterPop.js**, a lightweight toast notification library designed for modern web applications. With a size of less than 100KB and no dependencies, ButterPop.js allows you to create smooth, customizable notifications effortlessly. Explore the 23 beautiful themes and enjoy flexible positioning, progress indicators, and interactive elements.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Themes](#themes)
- [Customization](#customization)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Releases](#releases)

## Features

- **Lightweight**: Less than 100KB.
- **Zero Dependencies**: No need for external libraries.
- **Customizable**: Adjust colors, sizes, and positions.
- **Beautiful Themes**: Choose from 23 stunning designs.
- **Flexible Positioning**: Display notifications anywhere on the screen.
- **Progress Indicators**: Show progress for timed notifications.
- **Interactive Elements**: Include buttons for user actions.
- **Accessibility**: Designed with accessibility in mind.

## Installation

To get started with ButterPop.js, simply download the library from the [Releases](https://github.com/BAHEKARPRANAV/ButterPop.js/releases) section. You can choose the latest version and follow the instructions provided there.

Alternatively, you can add ButterPop.js to your project using a package manager. If you prefer npm, run:

```bash
npm install butterpop.js
```

If you use yarn, you can run:

```bash
yarn add butterpop.js
```

## Usage

Integrating ButterPop.js into your project is straightforward. Include the library in your HTML file:

```html
<script src="path/to/butterpop.js"></script>
<link rel="stylesheet" href="path/to/butterpop.css">
```

Once included, you can create a notification using the following code:

```javascript
ButterPop.show({
  title: 'Hello World!',
  message: 'This is a sample notification.',
  theme: 'default',
  duration: 3000
});
```

### Options

You can customize the notifications using various options:

- `title`: The title of the notification.
- `message`: The content of the notification.
- `theme`: Choose from available themes.
- `duration`: Set how long the notification should stay visible (in milliseconds).
- `position`: Define where the notification appears on the screen (top-right, bottom-left, etc.).

## Themes

ButterPop.js offers 23 unique themes to match your project's design. Some popular themes include:

- **Default**: A clean, minimalistic look.
- **Success**: Green tones for positive messages.
- **Error**: Red shades for alerts.
- **Info**: Blue hues for informational notifications.
- **Warning**: Yellow tones for cautionary messages.

You can easily switch themes by specifying the `theme` option when creating a notification.

## Customization

ButterPop.js allows for extensive customization. You can modify the styles in your CSS file to match your brand. Here are some common customizations:

### Change Colors

To change the default colors of notifications, override the CSS variables in your stylesheet:

```css
:root {
  --butterpop-success-color: #4CAF50;
  --butterpop-error-color: #F44336;
  --butterpop-info-color: #2196F3;
  --butterpop-warning-color: #FF9800;
}
```

### Adjust Sizes

You can adjust the sizes of the notifications by modifying the padding and font sizes in your CSS:

```css
.butterpop {
  padding: 15px;
  font-size: 16px;
}
```

### Add Custom Icons

You can include custom icons in your notifications by modifying the HTML structure in your JavaScript code:

```javascript
ButterPop.show({
  title: 'Custom Icon',
  message: 'This notification has a custom icon.',
  icon: 'path/to/icon.png'
});
```

## Examples

Here are some examples of how to use ButterPop.js effectively:

### Basic Notification

```javascript
ButterPop.show({
  title: 'Welcome!',
  message: 'Thank you for visiting our site.',
  theme: 'default'
});
```

### Success Notification

```javascript
ButterPop.show({
  title: 'Success!',
  message: 'Your action was successful.',
  theme: 'success',
  duration: 5000
});
```

### Error Notification with Button

```javascript
ButterPop.show({
  title: 'Error!',
  message: 'Something went wrong.',
  theme: 'error',
  buttons: [
    {
      text: 'Retry',
      onClick: () => {
        console.log('Retry clicked');
      }
    }
  ]
});
```

## Contributing

We welcome contributions to ButterPop.js! If you would like to help improve the library, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your branch to your forked repository.
5. Submit a pull request.

Please ensure that your code adheres to our coding standards and includes appropriate tests.

## License

ButterPop.js is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Releases

For the latest updates and versions, visit the [Releases](https://github.com/BAHEKARPRANAV/ButterPop.js/releases) section. Here, you can download the latest version and find detailed release notes.

---

Thank you for using ButterPop.js! We hope it enhances your web applications with beautiful notifications. If you have any questions or feedback, feel free to reach out through the repository issues.