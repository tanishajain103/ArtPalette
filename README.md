# ArtPalette 🎨

ArtPalette is an AI-powered Neural Style Transfer web application that transforms ordinary photographs into artistic images.

The application combines the content of one image with the visual style of another image using a PyTorch-based neural style transfer model and provides an interactive Flask web interface.

## Features

- Upload a content image
- Upload an artistic style image
- Adjustable style strength
- AI-powered neural style transfer
- Real-time image preview
- Generated artwork display
- Responsive web interface
- Flask-based web application

## Technology Stack

- Python
- PyTorch
- TorchVision
- Flask
- Flask-WTF
- Flask-Bootstrap
- NumPy
- Pillow
- HTML
- CSS
- JavaScript

## How It Works

1. Upload a content image.
2. Upload a style image.
3. Adjust the style strength.
4. The VGG encoder extracts feature representations from the images.
5. Adaptive Instance Normalization combines the content and style features.
6. The trained decoder generates the stylized image.
7. ArtPalette displays the final artwork.

## Project Structure

```text
ArtPalette/
│
├── app.py
├── train.py
├── requirements.txt
├── Procfile
├── vgg_normalised.pth
│
├── experiment/
│   └── final_exp/
│       ├── decoder_final.pth
│       └── options.txt
│
├── utils/
│   ├── models.py
│   └── utils.py
│
├── templates/
│   └── index.html
│
├── static/
│   └── uploads/
│
├── examples/
│
└── .gitignore