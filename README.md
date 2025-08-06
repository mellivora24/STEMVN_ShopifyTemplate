# 🛍️ STEMVN Shopify Template
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Liquid](https://img.shields.io/badge/Liquid-7AB55C?style=for-the-badge&logo=shopify&logoColor=white)
![Shopify](https://img.shields.io/badge/Shopify-7AB55C?style=for-the-badge&logo=shopify&logoColor=white)

## 🛠️ Tech Stack

**CSS3**: Styling
**Shopify Liquid**: engine
**Vanilla JavaScript**: Interactive functionality

## 📁 Project Structure

```
ShopifyWEB/
├── 📁 assets/                   # Static assets
├── 📁 config/                   # Theme configuration
├── 📁 layout/                   # Layout templates
├── 📁 locales/                  # Translation files
├── 📁 sections/                 # Reusable sections
├── 📁 snippets/                 # Reusable components
└── 📁 templates/                # Page templates
```

## 🚀 Installation

### Prerequisites
- Node.js 16+
- Shopify CLI installed
- Shopify Partner account


## 🔧 Development

### Local Development

```bash
# Start development server
shopify theme dev

# Pull theme from store
shopify theme pull

# Push changes to store
shopify theme push

# Create new theme
shopify theme push --unpublished --theme-name "Your Theme Name"
```

### Code Organization

#### CSS Architecture
```css
/* CSS Custom Properties for theming */
:root {
  --color-primary: #121212;
  --color-secondary: #ffffff;
  --font-body: 'Helvetica Neue', sans-serif;
}
```

#### JavaScript Modules
```javascript
// Modern ES6+ modules
import { cart } from './cart.js';
import { search } from './search.js';
```

#### Liquid Components
```liquid
<!-- Reusable snippets -->
{% render 'card-product', product: product, show_vendor: true %}
```


## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

- **Email**: thanhquyet.freelancer@gmail.com
- **Documentation**: [Shopify Theme Development](https://shopify.dev/themes)
- **Issues**: [GitHub Issues](https://github.com/mellivora24/stemvn-shopify-template/issues)

## 🔄 Changelog

### v1.0.0 (2024-01-XX)
- ✨ Initial release based on Dawn 15.4.0
- 🌐 Added 50+ language support
- 🎨 Custom STEMVN branding
- ⚡ Performance optimizations
- ♿ Accessibility improvements

---

**Made by Quyet Thanh at STEMVN**