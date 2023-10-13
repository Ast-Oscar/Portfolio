---
title: Rewriting Filters and QrCode in C#
publishDate: 2021-05-10 00:00:00
img: ../../assets/miniature_1.jpg
img_alt: An extract from the program
description: |
  In second year, I wrote from scratch the image filters functions and QrCode class
tags:
  - C#
  - Windows Forms
---

*Our project consists of different classes to process an image, apply filters, create images (fractal or image concealment), generate QR codes version 1 or 2 or compress an image without using the already created librairies QrCode or Pixel.*

<h4>The filters functions</h4>
<p style="width: 100%">
  In order to simplify some functions, we decided to re-program a Pixel class. We apply a convolution between the convolution matrix of the chosen filter and our image. We have write black and white filters, enlarge, shrink, zoom in, mirror effect, rotate, etc.
</p>

<h4>Writing QrCode</h4>
<p style="width: 100%">
  To create QR Code in version 1 or 2, we will check if the sentence wrote is in the right length (< 47 char). Once done we convert it in parts of 11 bits and complete them if necessary, with 0s. With a few other steps between, we add at the end the correction chain of error of the chain of character with the **Reed Solomon algorithm**.
  Once done, we create the QR Code with a zigzag algorithm and apply a mask 0 with a XOR door, and Ta-dam, we have our QR Code. We also created the option to colour gradient the QR Code.
</p>

<h4>Problems encountered and how I fixed them</h4>
<p style="width: 100%">
  At first, I had quite the hard time coding the header of an image, which is composed of many elements. Once it was done, the project went smoothly with minor problems (Unitary tests, convolution matrixes, compression method) 
</p>

<h4>The program demonstration</h4>

<video controls width="100%" muted controlsList="nodownload">
  <source src="../../assets/qrcode_demo.mp4" type="video/mp4">
</video>
