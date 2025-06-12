# Sample Images Repository

A public repository containing sample images for testing and development purposes.

## 📁 Repository Structure

```
sample-images/
├── README.md
└── nature/
    ├── heic/
    │   ├── 3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.HEIC
    │   └── 991825f7-2cd0-444f-86f6-5815a4330948.HEIC
    ├── jpeg/
    │   ├── 3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.jpg
    │   └── 991825f7-2cd0-444f-86f6-5815a4330948.jpg
    └── png/
        ├── 3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.png
        └── 991825f7-2cd0-444f-86f6-5815a4330948.png
```

## 🖼️ Available Images

### Nature Collection
The repository contains nature-themed images in multiple formats:

#### HEIC Format (`nature/heic/`)
- **3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.HEIC** - High-efficiency format
- **991825f7-2cd0-444f-86f6-5815a4330948.HEIC** - High-efficiency format

#### JPEG Format (`nature/jpeg/`)
- **3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.jpg** - Standard JPEG format
- **991825f7-2cd0-444f-86f6-5815a4330948.jpg** - Standard JPEG format

#### PNG Format (`nature/png/`)
- **3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.png** - Lossless PNG format
- **991825f7-2cd0-444f-86f6-5815a4330948.png** - Lossless PNG format

## 🔗 Direct Access URLs

You can access these images directly using the following URLs:

### HEIC Images
```
https://raw.githubusercontent.com/athameem/sample-images/main/nature/heic/3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.HEIC
https://raw.githubusercontent.com/athameem/sample-images/main/nature/heic/991825f7-2cd0-444f-86f6-5815a4330948.HEIC
```

### JPEG Images
```
https://raw.githubusercontent.com/athameem/sample-images/main/nature/jpeg/3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.jpg
https://raw.githubusercontent.com/athameem/sample-images/main/nature/jpeg/991825f7-2cd0-444f-86f6-5815a4330948.jpg
```

### PNG Images
```
https://raw.githubusercontent.com/athameem/sample-images/main/nature/png/3e12e195-2a45-4b2a-90d6-72dc0bb30bfe.png
https://raw.githubusercontent.com/athameem/sample-images/main/nature/png/991825f7-2cd0-444f-86f6-5815a4330948.png
```

## 📋 Usage

### For Testing Applications
These images are perfect for:
- Testing image upload functionality
- Testing image processing pipelines
- UI/UX development and prototyping
- Automated testing scenarios
- API endpoint testing
- Format conversion testing
- Cross-platform compatibility testing

### Code Examples

#### JavaScript/Node.js
```javascript
// Fetch different format images for testing
const formats = ['heic', 'jpeg', 'png'];
const imageId = '3e12e195-2a45-4b2a-90d6-72dc0bb30bfe';

for (const format of formats) {
  const extension = format === 'jpeg' ? 'jpg' : format;
  const imageUrl = `https://raw.githubusercontent.com/athameem/sample-images/main/nature/${format}/${imageId}.${extension}`;
  const response = await fetch(imageUrl);
  const imageBlob = await response.blob();
  console.log(`Downloaded ${format} image:`, imageBlob.size, 'bytes');
}
```

#### Python
```python
import requests
import os

# Download images in different formats
formats = {
    'heic': 'HEIC',
    'jpeg': 'jpg', 
    'png': 'png'
}

image_id = '3e12e195-2a45-4b2a-90d6-72dc0bb30bfe'
base_url = 'https://raw.githubusercontent.com/athameem/sample-images/main/nature'

for format_dir, extension in formats.items():
    url = f'{base_url}/{format_dir}/{image_id}.{extension}'
    response = requests.get(url)
    
    if response.status_code == 200:
        filename = f'test_image.{extension}'
        with open(filename, 'wb') as f:
            f.write(response.content)
        print(f'Downloaded {format_dir} image: {filename}')
```

#### cURL
```bash
# Download all formats of the same image
IMAGE_ID="3e12e195-2a45-4b2a-90d6-72dc0bb30bfe"
BASE_URL="https://raw.githubusercontent.com/athameem/sample-images/main/nature"

# Download HEIC
curl -o "${IMAGE_ID}.HEIC" "${BASE_URL}/heic/${IMAGE_ID}.HEIC"

# Download JPEG
curl -o "${IMAGE_ID}.jpg" "${BASE_URL}/jpeg/${IMAGE_ID}.jpg"

# Download PNG
curl -o "${IMAGE_ID}.png" "${BASE_URL}/png/${IMAGE_ID}.png"
```

## 📝 File Formats

- **HEIC**: High Efficiency Image Container format
  - Modern image format with better compression than JPEG
  - Commonly used by Apple devices
  - Supports both single images and image sequences
  - Smaller file sizes with high quality

- **JPEG**: Joint Photographic Experts Group format
  - Widely supported lossy compression format
  - Excellent for photographs and complex images
  - Universal browser and application support

- **PNG**: Portable Network Graphics format
  - Lossless compression format
  - Supports transparency
  - Ideal for images with sharp edges and text
  - Larger file sizes but perfect quality retention

## 🚀 Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/athameem/sample-images.git
   cd sample-images
   ```

2. **Use images directly in your tests:**
   - Reference images by path for local testing
   - Use raw GitHub URLs for remote testing
   - Choose appropriate format for your use case
   - Copy images to your test fixtures directory

## 📊 Image Information

| Image ID | HEIC | JPEG | PNG | Category | Use Case |
|----------|------|------|-----|----------|----------|
| 3e12e195-2a45-4b2a-90d6-72dc0bb30bfe | ✅ | ✅ | ✅ | Nature | General testing, format comparison |
| 991825f7-2cd0-444f-86f6-5815a4330948 | ✅ | ✅ | ✅ | Nature | General testing, format comparison |

### Format Comparison Benefits
- **Same image, multiple formats**: Perfect for testing format conversion
- **Quality comparison**: Compare lossy vs lossless compression
- **Size optimization**: Test different compression ratios
- **Compatibility testing**: Ensure your app handles various formats

## 🎯 Format-Specific Use Cases

### HEIC Images
- Testing Apple ecosystem compatibility
- Modern format support validation
- Compression efficiency testing
- iOS/macOS application development

### JPEG Images
- Web development and browser compatibility
- Standard image processing workflows
- Legacy system compatibility
- Social media and sharing platforms

### PNG Images
- UI element testing with transparency
- Lossless quality requirements
- Graphics and logo testing
- Screenshot and documentation images

## 🤝 Contributing

Feel free to contribute additional sample images by:

1. Fork this repository
2. Add your images to appropriate directories following the structure:
   - `nature/heic/` for HEIC files
   - `nature/jpeg/` for JPEG files  
   - `nature/png/` for PNG files
3. Update this README with new image information
4. Submit a pull request

### Guidelines for New Images
- Maintain the organized directory structure
- Provide same image in multiple formats when possible
- Use consistent naming conventions
- Ensure images are appropriate for public use
- Add image details to the information table
- Consider adding new categories as subdirectories

## 📄 License

This repository is public and the images are available for testing purposes. Please ensure you have the right to use these images in your projects.

## 🔧 Common Use Cases

- **Web Development**: Testing image upload forms and galleries
- **Mobile App Development**: Testing image handling and display across formats
- **API Testing**: Validating file upload endpoints with different formats
- **Image Processing**: Testing compression, conversion, and manipulation
- **Performance Testing**: Load testing with various image sizes and formats
- **Automated Testing**: Consistent test data for CI/CD pipelines
- **Format Conversion**: Testing conversion between HEIC, JPEG, and PNG
- **Cross-Platform Development**: Ensuring compatibility across different systems

## 📞 Support

If you encounter any issues or need additional sample images, please:
- Open an issue in this repository
- Contact the repository maintainer
- Submit a pull request with improvements

---

**Repository URL**: `https://github.com/athameem/sample-images`
