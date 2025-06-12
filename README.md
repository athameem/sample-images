# Sample Images Repository

A public repository containing sample images for testing and development purposes.

## 📁 Repository Structure

```
sample-images/
├── README.md
├── 3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.HEIC
├── 991825f7-2cd0-444f-86f6-5815a4330948.HEIC
└── nature/
```

## 🖼️ Available Images

### Root Directory
- **3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.HEIC** - HEIC format image
- **991825f7-2cd0-444f-86f6-5815a4330948.HEIC** - HEIC format image

### Categories
- **nature/** - Directory for nature-themed images (currently empty)

## 🔗 Direct Access URLs

You can access these images directly using the following URLs:

```
https://raw.githubusercontent.com/athameem/sample-images/main/3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.HEIC
https://raw.githubusercontent.com/athameem/sample-images/main/991825f7-2cd0-444f-86f6-5815a4330948.HEIC
```

## 📋 Usage

### For Testing Applications
These images are perfect for:
- Testing image upload functionality
- Testing image processing pipelines
- UI/UX development and prototyping
- Automated testing scenarios
- API endpoint testing

### Code Examples

#### JavaScript/Node.js
```javascript
// Fetch image for testing
const imageUrl = 'https://raw.githubusercontent.com/athameem/sample-images/main/3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.HEIC';
const response = await fetch(imageUrl);
const imageBlob = await response.blob();
```

#### Python
```python
import requests

# Download image for testing
url = 'https://raw.githubusercontent.com/athameem/sample-images/main/3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.HEIC'
response = requests.get(url)
with open('test_image.heic', 'wb') as f:
    f.write(response.content)
```

#### cURL
```bash
# Download image using cURL
curl -o test_image.heic https://raw.githubusercontent.com/athameem/sample-images/main/3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.HEIC
```

## 📝 File Formats

- **HEIC**: High Efficiency Image Container format
  - Modern image format with better compression than JPEG
  - Commonly used by Apple devices
  - Supports both single images and image sequences

## 🚀 Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/athameem/sample-images.git
   cd sample-images
   ```

2. **Use images directly in your tests:**
   - Reference images by filename for local testing
   - Use raw GitHub URLs for remote testing
   - Copy images to your test fixtures directory

## 📊 Image Information

| Filename | Format | Size | Use Case |
|----------|--------|------|----------|
| 3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.HEIC | HEIC | TBD | General testing |
| 991825f7-2cd0-444f-86f6-5815a4330948.HEIC | HEIC | TBD | General testing |

## 🤝 Contributing

Feel free to contribute additional sample images by:

1. Fork this repository
2. Add your images to appropriate directories
3. Update this README with new image information
4. Submit a pull request

### Guidelines for New Images
- Use descriptive filenames when possible
- Organize images into appropriate subdirectories
- Include various formats (JPEG, PNG, HEIC, WebP, etc.)
- Ensure images are appropriate for public use
- Add image details to the table above

## 📄 License

This repository is public and the images are available for testing purposes. Please ensure you have the right to use these images in your projects.

## 🔧 Common Use Cases

- **Web Development**: Testing image upload forms and galleries
- **Mobile App Development**: Testing image handling and display
- **API Testing**: Validating file upload endpoints
- **Image Processing**: Testing compression, conversion, and manipulation
- **Performance Testing**: Load testing with various image sizes
- **Automated Testing**: Consistent test data for CI/CD pipelines

## 📞 Support

If you encounter any issues or need additional sample images, please:
- Open an issue in this repository
- Contact the repository maintainer
- Submit a pull request with improvements

---

**Repository URL**: `https://github.com/athameem/sample-images`
